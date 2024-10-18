<script>
  import Step from "./Step.svelte";
  let steps = [
    {
      name: "Workout Track",
      icon: "fa-solid fa-list-check",
      description:
        "Smoljames Store is a a merchanising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.",
    },
    {
      name: "Labelle Sneakers",
      icon: "fa-solid fa-cart-shopping",
      description:
        "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
    },
    {
      name: "Roomé",
      icon: "fa-solid fa-diagram-project",
      description:
        "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
    },
  ];
  let benefits = [
    {
      metric: "10x",
      name: "a self taught developer",
      description:
        "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript and Typescript frameworks, React and Svelte, .",
    },
    {
      name: "Software Q/A Automation and Manual Tester",
      description:
        "Carefully crafting and designing Test Scenerios and Test Cases allows me to express and experiment with every morsel of Curiosity and Attention I have in me. I love the challenge giving users the best experience there is, assessing software products, hence my efficient knowledge in cypress, selenium and other automation tools.",
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
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="poppins text-violet-400">Judith </span> Omosehin..
        <br />A Frontend Developer/<span class="poppins text-violet-400"
          >Software Automation Q/A Engineer</span
        >
      </h2>

      <h3>
        My <b class="">Areas of Specialization as A Frontend Developer</b>:
        Javascript, typescript, React, Svelte/Sveltekit..
      </h3>

      <h3>
        My Areas of Specialization as A Software Tester <span
          >Cypress, Selenium, postman, API testing, PostgreSQL!
        </span>
      </h3>
      <a
        class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer ml-2"
        href="/"
        target="_blank"
      >
        <div
          class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
        ></div>
        <a class="relative z-9" href="tel:=08027228798">Get in touch</a>
      </a>
    </div>
    <div class="relative shadow-2xl grid place-items-center bg-cyan-700">
      <img
        src={"images/img1.jpg"}
        alt="Profile image"
        class="object-cover z-[2] max-h-[70vh]"
      />
    </div>
  </section>
  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-lg sm:text-xl md:text-2xl">
        A link to my Software Test Automation Repo..
      </h6>
      <h3>
        And of course <span class="poppins text-violet-400"
          >Test Cases and
        </span>Test scenerios I Have Designed..
      </h3>
    </div>
    <a
      href="https://https://github.com/judithprofprofile"
      target="_blank"
      class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
    >
      <i class="fa-regular fa-circle-play"></i>
      <p>Click</p>
    </a>
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>
          Workout Track Application, A companion for workout sessions and
          helpful when keeping tracks of your location and number of
          minutes/hours spent during workout<strong class="text-violet-800"
            >Html, Css, Javascript!</strong
          >
        </p>
      </Step>
      <Step step={steps[1]}>
        <p>
          Labelle Sneakers<strong class="text-violet-800">Svelte</strong>,
          <strong class="text-violet-800">Svelte, Typescript</strong>
          & <strong class="text-violet-800">TailwindCSS</strong> A functional application
          that saves you the stress of having to wait for a customer to compile your
          sneaker orders when you can just click the items you want..
        </p>
      </Step>
      <Step step={steps[2]}>
        <p>
          Pokédex
          <strong class="text-violet-800">Svelte</strong>,
          <strong class="text-violet-800">Svelte, Typescript</strong>
          & <strong class="text-violet-800">TailwindCSS</strong> A functional application
          that saves you the stress of having to wait for a customer to compile your
          sneaker orders when you can just click the items you want..
        </p>
      </Step>
    </div>
  </section>
  <section
    id="about"
    class="py-20 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
  >
    <div
      class="flex flex-col gap-2 text-center relative before:relative before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:relative after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700"
    >
      <h6 class="text-lg sm:text-xl md:text-2xl">Want to Know More?</h6>
      <h3 class="Font-semibold text-3xl sm:text-4xl md:text-5xl">
        A bit <span class="poppins text-violet-400">about</span>me.
      </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
      I am...
    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
        <div class="flex gap-6 sm:gap-8">
          <p
            class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-700 font-semibold"
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

    <div
      class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
    >
      <table class="bg-slate-300 text-slate-700 rounded text-center">
        <thead class="border-b border-solid border-slate-300">
          <tr>
            <th />
            <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
            <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
            <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
            <th class="whitespace-nowrap bg-cyan-700 text-white p-4 px-8">Me</th
            >
          </tr>
        </thead>
        <tbody>
          <tr>
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Dedication</td
            >
            <td><i class="fa-solid fa-check text-green-500"></i></td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-check text-green-500"></i></td>
            <td><i class="fa-solid fa-check text-green-500"></i></td>
          </tr>
          <tr>
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Thinking Ability</td
            >
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-check text-green-500"></i></td>
            <td><i class="fa-solid fa-check text-green-500"></i></td>
            <td><i class="fa-solid fa-check text-green-500"></i></td>
          </tr>
          <tr>
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Skills</td
            >
            <td><i class="fa-solid fa-check text-green-500"></i></td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-check text-green-500"></i></td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
      <p>scroll up to see more &rarr;</p>
    </div>
    <p class="mx-auto">So why not invest?</p>
  </section>
</main>
