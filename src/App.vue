<template>
  <div class="flex flex-col min-h-screen">
    <TopBar />
    <div class="flex flex-1 w-full">
      <RouterView />
    </div>
  </div>
</template>

<script setup>
import TopBar from "./components/TopBar.vue";
</script>
