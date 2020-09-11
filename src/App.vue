<template>
  <div id="app">
    <HeaderBlock />
  </div>
</template>

<script>
import HeaderBlock from './components/HeaderBlock.vue';

export default {
  name: 'App',
  components: {
    HeaderBlock
  },
  data: function() {
    return {

    }
  },
}
</script>

<style>
  * {
    box-sizing: border-box;
  }
  html {
    font-size: 10px;
  }
  body {
    background-color: #111;
    margin: 0;
    padding: 0;
  }
  #app {
    margin: 0 auto;
    font-family: 'Rubik Mono One', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #fffff3;
    overflow: hidden;
  }
</style>
