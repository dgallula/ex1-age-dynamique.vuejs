<template>
  <div class="ul">liste</div>
  <ul>
    <li> {{ persona.firstname }}</li>
    <li> {{ persona.lastname }}</li>
    <li> {{ persona.age }}</li>

    <button @click="randomAge">change age</button>
  </ul>
</template>

<script setup>
import { ref } from 'vue'

const persona = ref({
  firstname: 'John',
  lastname: 'Doe',
  age: 30
})
function randomAge() {
  persona.value.age = Math.floor(Math.random() * 100)
}
</script>

<script>
function randomAge() {
  persona.value.age = Math.floor(Math.random() * 100)
}
</script>



<style>
/* Ton style CSS */
</style>



