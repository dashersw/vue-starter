<script setup>
import { reactive } from "vue";

defineProps({
  msg: {
    type: String,
    required: true,
  },
});

const state = reactive({
  count: 0,
});

const increment = () => {
  state.count++;
};

const decrement = () => {
  state.count--;
};

const reset = () => {
  state.count = 0;
};
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      You’ve successfully created a project with
      <a href="https://vitejs.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>.
    </h3>
    <p>Now, let’s see what you can do with it.</p>
    <p>{{ state.count }}</p>
    <p>
      <button @click="increment">+</button>
      <button @click="decrement">-</button>
      <button @click="reset">reset</button>
    </p>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
