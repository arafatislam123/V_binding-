<script setup>
import { ref } from 'vue'
const color = ref("gray")
const textSize = ref("10")
const fontColor = ref("red")
</script>

<template>
  <button class="font-bold py-2 px-4 rounded" 
    :class="`bg-${color}-500 hover:bg-${color}-700`"
    :style="`font-size:${textSize}px; color:${fontColor}`"
  >
    Button
  </button>

  <div class="mt-20">
    <input class="border border-gray-300 p-2" type="text" v-model="color" placeholder="color"/>
    <input class="border border-gray-300 p-2" type="text" v-model="textSize" placeholder="textSize"/>
    <input class="border border-gray-300 p-2" type="text" v-model="fontColor" placeholder="fontColor"/>
  </div>
</template>

<style scoped>
</style>