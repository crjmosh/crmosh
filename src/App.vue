<template>
  <div id="app">
    <HeaderBlock />
    <AboutMe />
  </div>
</template>

<script>
import HeaderBlock from './components/HeaderBlock.vue';
import AboutMe from './components/AboutMe.vue';

export default {
  name: 'App',
  components: {
    HeaderBlock,
    AboutMe
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
  .section-dark {
    background-color: #111;
    color: #fffff3;
  }
  .section-light {
    background-color: #fffff3;
    color: #111;
  }
</style>
