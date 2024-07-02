<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div class="flex flex-col items-center justify-center min-h-screen bg-gray-100">
    <h1 class="text-4xl font-bold text-blue-600 mb-6">{{ msg }}</h1>

    <div class="card bg-white shadow-lg rounded-lg p-6 mb-6">
      <button
        type="button"
        @click="count++"
        class="w-full bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600 transition-colors"
      >
        Count is {{ count }}
      </button>
      <p class="mt-4 text-gray-700">
        Edit <code class="bg-gray-200 px-1 rounded">components/HelloWorld.vue</code> to test HMR
      </p>
    </div>

    <p class="mb-4 text-gray-600">
      Check out
      <a
        href="https://vuejs.org/guide/quick-start.html#local"
        target="_blank"
        class="text-blue-500 hover:underline"
        >create-vue</a
      >, the official Vue + Vite starter
    </p>
    <p class="mb-4 text-gray-600">
      Learn more about IDE Support for Vue in the
      <a
        href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support"
        target="_blank"
        class="text-blue-500 hover:underline"
        >Vue Docs Scaling up Guide</a
      >.
    </p>
    <p class="text-gray-500">
      Click on the Vite and Vue logos to learn more
    </p>
  </div>
</template>
