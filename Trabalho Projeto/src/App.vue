<script>
import { RouterView, RouterLink } from "vue-router";
export default{ components: RouterView,RouterLink};
</script>
<template>
<header>
  <div class="titulo">
  <h1>Cabeçalho</h1>
  </div>
  <div class="home">
  <router-link to="/">Home</router-link>
  </div>
  <div class="sobre">
  <router-link to="/about">Sobre</router-link>
  </div>

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
  background: #F2E5CA;
}
header{
 background: #0E6B88;
}
main{
  height: 250vh;
  background: #F2E5CA;;
}
.titulo{
  text-align: left;
}
.home{   float: left;
    border: none;
    padding: 0px;
    padding-left: 50px;
    width: 200px;
    font-family: Arial, Helvetica, sans-serif white;
}
  
.sobre{
    float: left;
    border: none;
    padding: 0px;
    width: 200px;}



  </style>