<script>
  import Icons from "./Icons.svelte";
  const features = [
    {
      title: "Cross Platform",
      desc: 'thanks to electron.js, "goje" can be installed on windows, linux and mac. (mac version still under development)',
      icon: "monitor",
    },
    {
      title: "Specefic",
      desc: '"goje" specificly was created to help fruit stores',
      icon: "check",
    },
    {
      title: "A lot of widgets",
      desc: "handy features that help you calculate your things",
      icon: "tool",
    },
    {
      title: "Pdf Export",
      desc: "reports will be represented as pdf so you can share/print it where ever u want ;)",
      icon: "pdf",
    },
    {
      title: "Backup",
      desc: "with backup option you can backup your data and in can of fire you can only be worry about fire it self not the data that miht be burning :)",
      icon: "database",
    },
  ];
</script>

<section>
  <div id="features" class="w-full flex justify-center items-center">
    <div class="grid md:grid-cols-2 lg:grid-cols-3 grid-cols-1 gap-4 w-3/4">
      {#each features as feature}
        <div
          class="block rounded-xl border border-gray-800 bg-gray-900 shadow-xl"
        >
          <h3 class="flex items-center  p-5 pb-0 text-xl font-bold text-white">
            <span class="mr-2">
              <Icons name={feature.icon} />
            </span>
            {feature.title}
          </h3>
          <p class="p-5 pt-2 pr-10 text-sm text-gray-300">{feature.desc}</p>
        </div>
      {/each}
    </div>
  </div>
</section>
