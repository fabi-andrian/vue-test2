<template>
<ul>
  <li>{{ person.firstName }}</li>
  <li>{{ person.lastName }}</li>
  <li>{{ person.age }}</li>
</ul>
<button @click.prevent="randomAge">Changer l'âge</button>
</template>

<script setup>
import { ref } from 'vue';
const person = ref ({
  firstName: 'Pablo',
  lastName: 'Escobar',
  age:  30,
})
const randomAge = () => {
  person.value.age = Math.round(Math.random() * 100)
  }
</script>