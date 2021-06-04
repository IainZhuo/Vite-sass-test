<template>
  <h2>Hello Vue 3.0 + Vite.</h2>
  <p>
    <span>Count is: {{ count }} &nbsp;&nbsp;</span>
    <button @click="setCount(count + 1)">increment</button>
  </p>
</template>

<script>
import { useState } from 'vue3-hooks';

export default {
  name: 'App',
  setup() {
    const [count, setCount] = useState(0);

    return {
      count,
      setCount,
    };
  },
};
</script>

<style>
@import './index.scss';
h2 {
  color: teal;
}
</style>

