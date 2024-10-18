<script>
  export let y;

  let tabs = [
    { name: "Projects", link: "#projects" },
    { name: "About me", link: "#about" },
  ];
</script>

<header
  class={"sticky z-[10 top-0 duration-200 px-6 flex items-center justify-between border border-solid " +
    (y > 0
      ? "py-4 bg-cyan-600 border-cyan-600"
      : "py-8 bg-transparent border-transparent")}
>
  <h1 class="font-medium">
    <b class="font-bold poppins">Services</b>
  </h1>
  <div class="sm:flex items-center gap-4 hidden">
    {#each tabs as tab, index}
      <a href={tab.link} class="duration-200 hover:text-violet-400">
        <p>{tab.name}</p>
      </a>
    {/each}

    <a
      href="/"
      target="_blank"
      class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950"
    >
      <div
        class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
      ></div>

      <a class="relative z-9" href="tel:=08027228798">Get in touch</a>
    </a>
  </div>
</header>
