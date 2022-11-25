<script>
import { mapActions, mapState } from "pinia";
import { useCounterStore } from "../stores/counter";

export default {
  computed: {
    ...mapState(useCounterStore, ["count", "doubleCount"]),
  },
  methods: {
    ...mapActions(useCounterStore, ["increment"]),
  },
};
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    <p>{{ count }}</p>
    <p>{{ doubleCount }}</p>
    <button @click="increment">+</button>
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
