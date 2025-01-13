<!-- Interactive counter component -->
<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)
const increment = () => count.value++
const decrement = () => count.value--
</script>

<template>
  <div class="flex items-center space-x-4">
    <button 
      @click="decrement"
      class="px-4 py-2 bg-red-500 text-white rounded-lg hover:bg-red-600 transition"
    >
      -
    </button>
    <span class="text-2xl font-bold">{{ count }}</span>
    <button 
      @click="increment"
      class="px-4 py-2 bg-green-500 text-white rounded-lg hover:bg-green-600 transition"
    >
      +
    </button>
  </div>
</template>