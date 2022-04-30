<template>
  <div>
    <h1>{{ msg }}</h1>
    <button @click="handleCount">count: {{ count }}</button>
  </div>
</template>

<script setup>
  import { ref } from '@vue/composition-api'
  const msg = ref('Hello, Vue2 + Vite + CompositionAPI')
  const count = ref(0)

  function handleCount() {
    count.value += 1
  }
</script>
