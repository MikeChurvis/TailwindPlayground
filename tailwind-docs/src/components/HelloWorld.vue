<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <p>
    Recommended IDE setup:
    <a href="https://code.visualstudio.com/" target="_blank">VSCode</a>
    +
    <a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
  </p>

  <p>
    See
    <code>README.md</code> for more information.
  </p>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">Vite Docs</a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Docs</a>
  </p>

  <button
    type="button"
    @click="count++"
    class="border border-slate-700 rounded-lg p-2 m-2 shadow-lg active:mb-1.5 active:mt-2.5 active:shadow-sm"
  >count is: {{ count }}</button>
  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<style scoped>
h1 {
  @apply font-bold text-3xl;
}

a {
  /* color: #42b983; */
  @apply text-green-500 
  hover:text-green-400 hover:border-b hover:border-green-400 
  visited:text-green-600;
}

label {
  /* margin: 0 0.5em;
  font-weight: bold; */
  @apply my-0.5 font-bold;
}

code {
  /* background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455; */
  @apply px-1.5 py-1 bg-slate-200 rounded-sm text-slate-700;
}
</style>
