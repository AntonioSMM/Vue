<script>
  export default{
    data: () => ({
      contador : 10,
    }),

  methods: {
    saludar (){
      console.log("hola 10A ");
     },
     incrementar() {
      this.contador++;
     },
     decrementar () {
      this.contador--;
     },
     resetear(){
      this.contador = 10;
     },
    }
  };
</script>



<template>
  <link rel = "stylesheet" href="base.css">
  <img src ="./assets/logo.svg" alt="Logo VUE" 
  width = "125" height="125">
  <div class ="container">
    <small>
      <h1> Hola desde VUE.js 3 </h1>
    </small>
  <hr>
  <h2>Contador {{ contador }}</h2>
  <button v-on:click="incrementar()"> +1 </button>
  <button @click="decrementar()">  -1 </button>
  <button @click="resetear ()"> reset </button>
  </div>
</template>





<style scoped>
 .container{
  text-align: center;
 }

 small{
  color: #666;
 }

 h1 {
  font-weight: bolder; 
  color: red;
 }

 h2 {
  font-size: 2.5rem;
 }

 button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 8px;

 }

</style>