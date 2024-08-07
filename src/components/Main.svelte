<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Beast Morph",
            icon: "fa-solid fa-dumbbell",
            href: "https://nithin-beast-morph.netlify.app/",
            },
        {
            name: "Facial Expression Recognition",
            icon: "fa-solid fa-network-wired",
            href: "https://github.com/NithinChowdaryRavuri/facial_expression_recognition",
            },
        {
            name: "Pokedex",
            icon: "fa-solid fa-mobile-screen",
            href: "https://nithin-pokedex.netlify.app/",
            },
        
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a passion driven developer",
            description:
            "Embarking from an Electronics background, I discovered my true passion lies in coding and product development. This led me to self-learn programming and subsequently earn a Master's in Computer Science. My skills, ranging from JavaScript frameworks to Python & Java, are showcased in my GitHub portfolio, reflecting a journey of continuous learning and a dedication to crafting innovative digital experiences.",
        },
        {
            name: "data structures & algorithms finatic",
            description:
            "Through the digital terrain of LeetCode, I've battled over 400 problems, each one a step towards mastery in data structures and algorithms. My daily conquests are not just for personal glory—they're shared with the world in my GitHub repository, a showcase of persistence and skill in code.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h1 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Nithin Chowdary</span> Ravuri
                <br />Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h1>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> favorite tech</span> includes JavaScript
                (NEXT.JS or SvelteKit), TailwindCSS, Node.js + Express.js & PostgreSQL
                or Firebase/Firestore!
            </p>
            <a href="https://nithin-chowdary-portfolio.netlify.app/" target="_blank"
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Download my resume &darr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[60vh]"
            />
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href="https://github.com/NithinChowdaryRavuri"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
        <i class="fa-brands fa-github"></i>
            <p>Github</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    The Beast Morph is a <strong class="text-violet-400"
                        >ReactJs, TailwindCSS</strong
                    >
                    web application, hosted on
                    <strong class="text-violet-400">Netlify</strong>, that
                    is designed for <strong class="text-violet-400">gym-goers</strong> of all levels, ensuring an
                    effective workout experience with essential features and seamless responsiveness on any device.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Facial Expression Recognition is an innovative deep learning application powered by 
                    <strong class="text-violet-400">CNN</strong> and 
                    <strong class="text-violet-400">OpenCV</strong>. 
                    It boasts the ability to interpret facial expressions in real-time, utilizing a 
                    pre-trained model to bring a new level of interactivity to user experiences.

                </p>
            </Step>
            <Step step={steps[2]}>               
                <p>
                    The Pokedex is a web application crafted with <strong class="text-violet-400">ReactJS</strong> 
                    and styled using <strong class="text-violet-400">TailwindCSS</strong>, proudly hosted on 
                    <strong class="text-violet-400">Netlify</strong>. It taps into the 
                    vast <strong class="text-violet-400">Poke API</strong> to showcase an extensive collection of Pokémon. 
                    Each Pokémon beckons with a click, revealing a world of details for enthusiasts and trainers alike.
                </p>
            </Step>
            <!-- <Step step={steps[2]}>               
                <p>
                    The NASA APOD is a  <strong
                        class="text-violet-400"
                        >ReactJS</strong
                    > web application hosted on
                    <strong class="text-violet-400">Netlify</strong>, that consumes the 
                    <strong class="text-violet-400">NASA API</strong> to display the
                    Astronomy Picture of the Day. It's a great way to learn about
                    the cosmos and the universe we live in.
                </p>
            </Step> -->
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap rounded p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
</main>