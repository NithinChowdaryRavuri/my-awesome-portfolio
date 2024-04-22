<script>
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Header from "../components/Header.svelte";

  let y;
  let innerHeight=0;
  let innerWidth=0;

  function goTop() {
    document.body.scrollIntoView({behavior: 'smooth'})
  }
</script>

<div class='relative flex flex-col max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen'>
  <div class={'fixed bottom-10 right-5 mr-20 w-full duration-200 flex z-[10] '+(
    y>0 ? 'opacity-full pointer-events-auto' : 'opacity-0 pointer-events-none'
  )} >
    <button on:click={goTop} class='ml-auto rounded-full bg-slate-900 
    text-violet-400 px-3 sm: px-4 hover:bg-slate-800 cursor-pointer hidden sm:block' >
      <i class='fa-solid fa-arrow-up grid place-items-center aspect-square'/>
    </button>
  </div>
  <Header y={y}/>
  <slot/>
  <Footer/>
</div>

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth/>