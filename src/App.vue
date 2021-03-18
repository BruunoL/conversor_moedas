<template>
  <div id="app">
    <h1>Conversor de Moedas</h1>
    <div class="box">
        <Conversor moeda-a="USD" moeda-b="BRL"></Conversor>
        <Conversor moeda-a="EUR" moeda-b="BRL"></Conversor>
        <Conversor moeda-a="JPY" moeda-b="BRL"></Conversor>

        <Conversor moeda-a="BRL" moeda-b="USD"></Conversor>
        <Conversor moeda-a="BRL" moeda-b="EUR"></Conversor>
        <Conversor moeda-a="BRL" moeda-b="JPY"></Conversor>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";

export default {
  name: 'App',
  components: {
    Conversor
  }
}
</script>

<style>
body {
    font-family: 'Saira Condensed',sans-serif;
}

#app h1 {
  text-align: center;
      background: linear-gradient(to top right,#ff2a00 0,#ffb600 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.box {
  max-width: 1000px;
  margin: 0 auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 30px;
  display: flex;
  flex-wrap: wrap;
}
</style>
