<template>
<ul>
  <li>{{ person.firstName }}</li>
  <li>{{ person.lastName }}</li>
  <li>{{ person.age }}</li>
</ul>
</template>

<script setup>
import { ref } from 'vue';
const person = ref ({
  firstName: 'Michael',
  lastName: 'Jackson',
  age:  50,
})
</script>