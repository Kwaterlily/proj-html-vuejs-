<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <TheHeader />
    <TheJumbotron />
    <TheFooter />
    <BaseFooterBelow />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import TheHeader from './components/TheHeader.vue';
import TheJumbotron from './components/Thejumbotron.vue';
import TheFooter from './components/TheFooter.vue';
import BaseFooterBelow from './components/BaseFooterBelow.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    TheHeader,
    TheJumbotron,
    TheFooter,
    BaseFooterBelow
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
