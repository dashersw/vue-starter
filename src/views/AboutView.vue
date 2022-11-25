<script setup>
import { useCounterStore } from "../stores/counter";

const store = useCounterStore();
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <p>{{ store.count }}</p>
    <p>{{ store.doubleCount }}</p>
    <button @click="store.increment">+</button>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
