<template>
  <h1 class="titulo">{{title}}</h1>
  <div>
  <button @click="helloWorld()" :class="clases">CLICK ME!</button>  
  </div>


</template>

<script setup>
import { ref } from 'vue';


const helloWorld = () =>{
  alert('Hello World')
}
const title = ref('Hello World')

const clases = ['text', 'bg'];
</script>

<style scoped>

.titulo{
  background-color:yellowgreen;
  font-weight: bold;
  padding: 25px;

}

.text{
  font-style: italic;
  font-size: 25px;
}
.bg{
  background-color: blueviolet;
}
</style>