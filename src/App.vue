<script setup>
import { ref } from "vue"
const count = ref(0)

const incCount = () => {
  count.value = count.value + 1
}

const decCount = () => {
  count.value = count.value - 1
}
</script>


<template>
  <main>
    <div>
      <h2>Current count is...</h2>
      <h1>{{ count }}</h1>
      <button @click="decCount()">-</button>
      <button @click="incCount()">+</button>
    </div>
  </main>
</template>


<style scoped>
  main{
    background-color: gray;
    display: flex;
    height: 100vh;
    width: 100vw;
    justify-content: center;
    align-items: center;
  }

  div{
    text-align: center;
  }
</style>
