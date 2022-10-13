<!-- TEMPLATE -->
<template>
  
<Navbar />
<br>
<!-- Iteration 2 | Display the result of a Javascript operation in a 
  component's HTML -->

<div>
2 + 2 = {{sumNumbers(2, 2)}} <br>
2 + 2 = {{2+2}}
</div>
<div>
  {{printString('This is a string printed by a function.')}} <br>
  {{'This is a String printed directly.' }}
</div>

<!-- ITERATION 3: create a boolean data inside a Vue component, and link it to 
  an HTML element that will only show up in your template if the 
  condition is set to true. -->

  <h3 v-if="correcto">Iteration 3 completed!</h3>



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
const correcto = ref(true)


</script>

<!-- STYLE -->
<style>


</style>
