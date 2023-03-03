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
    <button @click='count = 0'> D</button>
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
  background-size: cover;
}
.center{
  text-align: center;
}
button {
  margin-right: 10px;
  border-radius: 15px;
  border: 1px solid white;
  background-color: black;
  color: white;
  width: 20px;
  height: 20px;
  align-items: center;
  text-align: center;

}
button:hover{
  color: yellow;
  cursor: pointer;
}
</style>
