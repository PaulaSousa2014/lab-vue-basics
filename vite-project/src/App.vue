<!-- TEMPLATE -->
<template>
  
<Navbar />
<br>
<div>

2 + 2 = {{sumNumbers(2, 2)}} <br>
2 + 2 = {{2+2}}
</div>
<div>
  {{printString('This is a string printed by a function.')}} <br>
  {{'This is a String printed directly.' }}
</div>
<Footer />

</template> 

<!-- SCRIPT COMPOSITION API (JavaScript)-->
<script setup>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

import { ref } from 'vue'
const num1 = ref(Number)
const num2 = ref(Number)
const sumNumbers = (num1, num2) => {
    return num1 + num2;
}

const name = ref(String)
const printString = (name) => {
  return name
}



</script>

<!-- STYLE -->
<style>


</style>
