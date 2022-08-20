<template>
  <div class="about">
    <About />
  </div>
</template>

<script setup lang="ts">
import About from "@/components/About.vue";
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 90vh;
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    align-items: flex-start;
  }
}
</style>
