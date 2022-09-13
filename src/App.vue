
 
<script>
 

  export default{
    data:() => ({
      contador:500,
    }),
    methods:{
      saludar(){
        console.log("hola 4A");
      },
      incrementar(){
        this.contador++;
      },
      decrementar(){
        this.contador--;
      },
      resetear(){
        this.contador=500;
      },
    }
  };
</script>
<template>
  <img src="./assets/logo.svg" alt="logo vue" width="125" height="125">
  <div class="container">
    <small>
      <h1>Hola desde VUE.13</h1>
    </small>
    <br>
    <h2>Contador {{contador}}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="resetear()">reset</button>
    <br>
    Citlally Itzel Carrera Sanchez
    

  </div>
</template>

<style scoped>
  .container{
    text-align:center;
  }
  small{
    color:#666;
  }
  h1{
    font-weight:bolder;
  }
  h2{
    font-size: 2.5rem;
  }
  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 8px;
  }
</style>