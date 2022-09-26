<script>
  export default{
    data: () => ({
      contador: 10,
    }),
    methods: {
      saludar(){
        console.log ("Hola 10A")
      },
      incrementar() {
        this.contador++;
      },
      decrementar() {
        this.contador--;
      },
      resetear() {
        this.contador= 10;
      },

    }
     
  };
</script>
<template>
  <div class="navv">
    <ul class="nav justify-content-center " >
        <li class="nav-item">Jesus Flores Reyes</li>
        <li class="nav-item">4° "B"</li>
    </ul>
  </div>
  <div class="container">
    <img src="./assets/logo.svg" alt="LogoVUE" width="125" height="125">
    <small>
      <h1>Hola mundo desde VUE.JS 3</h1>
    </small>
    <hr>
    <h2>Contador {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="resetear()">Reset</button>
  </div>
</template>

<style scoped>
  
  
  h1{
    font-weight: bolder;
  }
  small{
    color: #666;
  }
  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 8px;
  }
  h2{
    font-size: 2.5rem;
  }

  li{
    margin-left: 100px;
  }
  .container{
  text-align: center;
  }
  div .navv{
    height: 30px;
    background: rgb(173, 77, 173);
  }
</style>