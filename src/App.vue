<script setup>
  import {ref} from "vue";

  const count = ref(0);
</script>

<template>
  <main>
    <div>
      <h4>
        The current count is...
      </h4>
      <h1>{{ count }}</h1>
      <button @click="count--">-</button>
      <button @click="count++">+</button>
    </div>
  </main>
</template>

<style scoped>
  main {
    background-color: aliceblue;
    height: 100vh;
    width: 100vw;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  div {
    text-align: center;
  }

  button {
    padding: 10px 40px;
    border: none;
    text-align: center;
    font-size: 20px;
    margin: 0 10px;
    cursor: pointer;
    color: white;
    background: black;
  }

   h1 {
    margin: 30px 0px;
    color: orangered;
    font-size: 60px;
    font-weight: bold;
  }

  h4 {
    background: black;
    padding: 10px 20px;
    color: white;
    font-weight: bold;
    font-size: 24px;
  }
</style>