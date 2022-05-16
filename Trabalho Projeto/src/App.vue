<script>
import { RouterView, RouterLink } from "vue-router";
export default{ components: RouterView,RouterLink};
</script>
<template>
<header>
  <h1>Cabeçalho</h1>
  <router-link to="/">Home</router-link>
  <router-link to="/about">Sobre</router-link>
</header>
<main><RouterView />
</main> 
<footer>rodape</footer>
</template>
<style>
body{
  margin: 0px;}
#app{
  height: 100vh;
}  
header, footer{
  height: 15%;
  margin: 1px solid black;
}
header{
  background-color: cyan ;
}
main{
  height: 250vh;
  background-color: blanchedalmond;
}


  </style>