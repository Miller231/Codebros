<template>
  <div>
    <h1>{{ message }}</h1>
    <button @click="increment">Click Me</button>
    <p>You've clicked the button {{ count }} times.</p>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const count = ref(0)
    const message = ref('Welcome to Vue 3 with Composition API!')

    function increment() {
      count.value++
    }

    return {
      message,
      count,
      increment
    }
  }
}
</script>

<style scoped>
h1 {
  color: #42b983;
}
</style>
