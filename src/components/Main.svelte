<script>
 import Step from "./Step.svelte";
 let steps = [
    {name: 'Calculator', icon:'fa-solid fa-calculator'},
    {name: 'Music player', icon:'fa-solid fa-music'},
    {name: 'Password Generator', icon:'fa-solid fa-lock'},
 ]
 let benefits = [
    {name: 'a self taught developer', description: 'I am a passionate self-taught developer with a strong drive for learning and building software. Through my own dedication and resourcefulness, I have acquired skills in HTML, CSS, JavaScript, SevelteKit, Tailwind CSS, Bootstrap, and Figma. Currently, I am expanding my knowledge by learning React and Vue.js, allowing me to create dynamic and interactive web applications.'},
    {name: 'a product design & marketing thinker', description: 'I am a passionate self-taught product design and marketing thinker. With a strong drive for learning and innovation, I have honed my skills in product design, user experience, and marketing strategies. My resourcefulness and dedication have allowed me to excel in creating compelling designs and implementing effective marketing campaigns. I am continuously expanding my knowledge and staying abreast of the latest trends and techniques in the field.'},
    {name: ' an excellent communicator', description: 'I am an excellent communicator, with the ability to effectively convey ideas and information. Through my strong verbal and written communication skills, I am able to articulate complex concepts in a clear and concise manner. I actively listen to others, foster open dialogue, and adapt my communication style to connect with diverse audiences.'},
 ]
</script>
<main class="flex flex-col flex-1 p4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-6xl">
                Hi! I'm <span class="text-violet-400"> Ali </span>El Slimani<br/> Front-End <span class="text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">favorite tech</span> includes HTML CSS & JavaScript(NEXT.JS or SveleKit, TailwindCSS or Bootstrap,)
            </p>
            <a href="https://www.linkedin.com/in/ali-slimani-2b4b74169/" target="_blank" class="blueShadow mx-auto lg:mr-auto  lg:ml-0 text-base sm:text-xl relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" >
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200">
                </div>
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img src={"https://scontent.frba3-2.fna.fbcdn.net/v/t39.30808-6/329352528_1425221198306239_2658665007343118912_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=efb6e6&_nc_eui2=AeH0zAI-6N-ee0QX0rq8RSisWPxZFNlOJXZY_FkU2U4ldl8ihI5uTLMrdtO4iL7tnfNqbKWzM1lKGgvTzhsotZX-&_nc_ohc=7LNZGlyTrt0AX-CKNPm&_nc_ht=scontent.frba3-2.fna&oh=00_AfBcPrpoNpQsoH7VxzH4QDufFDHRKHebWQ2AbFc37o6kSg&oe=65D98F5E"} alt="dashboard" class="object-cover z-[2] max-h-[70vh]"/>
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="text-violet-400">see</span> my work?
            </h3>
            
        </div>
        <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm: -mb-0 -mt-10 hover:border-violet-700 duration-200">
            <i class="fa-regular fa-circle-play"></i>
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step ={steps[0]}>
                    <p>Calculator is a <strong class="text-violet-400"> JavaScript</strong> Well crafted calculator where i was Working on my Technical aspect in the <strong class="text-violet-400">Arithmetics Operators</strong> Concepts</p>
            </Step>
            <Step step ={steps[1]}>
                <p>The Music Player is a <strong class="text-violet-400"> JavaScript</strong> Music Player where i was Working and Go deep on my Technical aspect in the <strong class="text-violet-400">Array Concepts & methods+ DOM manipulation and Objects</strong> concept </p>
            </Step>
            <Step step ={steps[2]}>
                <p>The Password Generator is a <strong class="text-violet-400"> JavaScript</strong> program that Generate Strong and powerful passwords its gives me deep understanding how the <strong class="text-violet-400">reGex and Loop </strong>combination could give me powerful ability in my programs 
            </Step>
        </div>
    </section>
    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl">Want to know More?</h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">A bit <span class="text-violet-400"> About</span> me.</h3>
        </div>
        <p class="mx-auto font-semibold text-lg sm:text-xl md:text-2xl">I am . . .</p>
        <div class="flex flex-col gap-20 w-full mx-auto mx-w-[800px]">
            {#each benefits as benefit, index }
            
            <div class="flex gap-6 sm:gap-8">
                <p class=" text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
                    0{index+1}
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
        <h5 class="text-2xl sm:text-3xl font-semibold text-center">The <span class="text-violet-400">Complete</span> Package</h5>
        <div class=" flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr class="">
                        <th/>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th class="whitespace-nowrap p-4 px-8 bg-violet-700 text-white">Me</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold whitespace-nowrap">Dedication</td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white  whitespace-nowrap pl-4 pr-8 py-4 font-semibold">Critical Thought</td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid whitespace-nowrap border-white pl-4 pr-8 py-4 font-semibold">Interpersonal Skills</td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold whitespace-nowrap">Programming Ability</td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p> Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not Invest</p>
    </section>
</main>