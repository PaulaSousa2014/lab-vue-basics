<template>
<!-- Iteration 4 | Display a list of elements that are stored inside
         a component 
        1. Create a list of posts inside the data of one of your Vue components. 
 These posts need to include the following data: title, description, and 
 content; and you need at least three of them. -->

<div v-for="user, index in clients" :key="index">
    <li>{{ user.client.name }}</li></div>
 
    
   
</template> 
<script setup>
import { ref } from 'vue'
const clients = [{ 
    client: {
        name: 'Andrea',
        title: 'Sra.',
        description: 'sfasfasf',
        content: 'sdfasfsf'
    }},
    {
        client: {
        name: 'Bruno',
        title: 'Sr.',
        description: 'sfasfasf',
        content: 'sdfasfsf'
    }},
    {
    client: {
        name: 'Jose',
        title: 'Sr.',
        description: 'sfasfasf',
        content: 'sdfasfsf'
    }

}]


</script> 
<style></style>