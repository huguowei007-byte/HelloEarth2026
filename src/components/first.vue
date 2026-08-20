<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <h1 :class="'title'">Make me red</h1>
  <button @click="increment">My Count is: {{ count }}</button>

</template>

<style>
.title {
  color: red;
}
</style>