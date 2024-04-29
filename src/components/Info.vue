<template>
  <div class="flex w-full gap-x-3 mb-5 p-3">
    <div class="pic" v-for="pic in 3">
      <img
        src="/2013_lexus_es-350_sedan_base_rq_oem_1_300.jpg"
        alt="pic-img"
        class="w-full rounded-xl"
      />
    </div>
    <div class="relative pic">
      <img
        src="/2013_lexus_es-350_sedan_base_rq_oem_1_300.jpg"
        alt="pic-img"
        class="w-full rounded-xl"
      />
      <div
        class="bg-[rgb(0,0,0,0.7)] pic absolute top-0 text-white font-light text-2xl flex items-center justify-center"
      >
        +110
      </div>
    </div>
  </div>

  <div class="flex w-full gap-x-3 bg-gray-200 w-max rounded-xl p-3">
    <div
      class="aspect-video w-44 rounded-md bg-white flex flex-col justify-center items-center"
      v-for="data in highLights"
      :key="data.text"
    >
      <h2 class="font-semibold text-gray-900">24 mpg</h2>
      <p class="font-light text-gray-700">combined MPG</p>
    </div>
  </div>

  <div>
    <h3>Edmunds' Expert Review</h3>
    <h6>by <span> the Edmunds Experts </span></h6>

    <h4>Pros</h4>
    <div class="flex" v-for="i in 3">
      <i>i</i>
      <p>Velvety-smooth V6 engine</p>
    </div>

    <h4>Cons</h4>
    <div class="flex" v-for="i in 3">
      <i>x</i>
      <p>
        Mouse-based electronics interface can be cumbersome and distracting to
        use.
      </p>
    </div>

    <h4>What’s new</h4>
    <p>
      The 2014 Lexus ES 350 now comes standard with HID headlights, while the
      standard foglights now use LED bulbs. In addition, sedans with the NuLuxe
      leatherette upholstery can now be equipped with ventilated seats as an
      option, and bamboo wood interior trim is a new alternative to the
      customary maple trim. Finally, the Display Audio package picks up Siri
      Eyes Free compatibility for newer iPhone owners.
    </p>
    <h4>Edmunds says</h4>
    <p>
      The 2014 Lexus ES 350 remains the standard-bearer for a relaxed,
      luxuriously insulated form of transportation. The competition has narrowed
      the gap over the years, though, so it's hardly your only option for an
      entry-level luxury sedan.
    </p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      highLights: [
        { heading: "", text: "" },
        { heading: "", text: "" },
        { heading: "", text: "" },
        { heading: "", text: "" },
      ],
    };
  },
};
</script>

<style>
.pic {
  @apply aspect-video w-44 rounded-xl;
}
</style>
