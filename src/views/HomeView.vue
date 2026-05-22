<template>
  <div
    class="flex flex-col py-12 items-center justify-center h-full w-full border"
  >
    <input
      v-model="search"
      type="text"
      placeholder="Digite o game"
      class="flex p-4 border w-110 h-12 m-5 items-center justify-center"
    />
    {{ search }}
    <main class="border grid grid-cols-3 place-items-center gap-8 p-8 w-[75%]">
      <Card v-for="n in 9" />
    </main>
  </div>
</template>

<script>
import Card from "../components/Card.vue";

export default {
  name: "HomeView",

  data() {
    return {
      search: "",
    };
  },

  components: {
    Card,
  },
};
</script>
