<script setup>
import { ref } from 'vue';
let count = ref(0);
</script>


<template>
  <div class="container">
    <div class="center">
    <h4>
      The Current count is... 
    </h4>
    <h1>{{ count }}</h1>
    <button @click='count++'>+</button>
    <button @click='count--'>-</button>
  </div>
  </div>
</template>

<style scoped>
.container {
  width: 100vw;
  height: 100vh;
  background-color: black;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}
.center{
  text-align: center;
}
</style>
