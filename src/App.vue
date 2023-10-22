<script lang="ts">
export default {
  data: () => ({
    contador: 0,
  }),
  methods: {
    aumentar(){
      this.contador++;
    },
    disminuir(){
      this.contador--;
    },
    resetear(){
      this.contador = 0;
    },
  }
}
</script>

<template>
  <div class="contenedor">
    <img src="./assets/logo.svg" alt="logo Vue" />
    <h1>Hello VueJS</h1>
    <h2>Contador: {{ contador }}</h2>
    <button @click="aumentar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="resetear()">Resetear</button>
  </div>
</template>

<style scoped>
    img {
      width: 100px;
      height: 200px;
  }

    .contenedor{
      text-align: center;
    }

</style>
