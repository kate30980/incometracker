<template>
  <Header />
</template>

<script>
import { reactive, computed } from 'vue';
import Header from './components/Header'

export default {
  setup(){
    return{ 
      Header
    }
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', sans-serif;
}
body{
  background-color: #eee;
}
</style>
