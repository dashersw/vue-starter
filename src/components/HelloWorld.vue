<script>
export default {
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    },
    reset() {
      this.count = 0;
    },
  },
};
</script>

<template lang="pug">
.greetings
  h1.green {{ msg }}
  h3 You’ve successfully created a project with&nbsp;
    a(href='https://vitejs.dev/' target='_blank' rel='noopener') Vite
    |  +&nbsp;
    a(href='https://vuejs.org/' target='_blank' rel='noopener') Vue 3
    | .
  p Now, let’s see what you can do with it.
  p {{ count }}
  p
    button(@click='increment') +
    button(@click='decrement') -
    button(@click='reset') reset
  slot
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
