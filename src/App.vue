<template>
  <div id="app">
    <TheHeader :links="menuLinks" />
    <TheJumbotron />
    <TheFooter />
    <BaseFooterBelow />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheJumbotron from './components/Thejumbotron.vue';
import TheFooter from './components/TheFooter.vue';
import BaseFooterBelow from './components/BaseFooterBelow.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheJumbotron,
    TheFooter,
    BaseFooterBelow,
  },
  data(){
    return{
      menuLinks: [
        { id: 1, url: "#", text: "Open Hours:", day: "Mon-Sat -", hour: "9:00 -18:00", active: false },
        { id: 2, url: "#", phone_icon: "tel:", number: "+1(305) 1234-5678", mail_icon: "mail", mail: "hello@example.com", f_icon: "facebook", t_icon: "twitter", l_icon: "linkedin", active: false }
      ]
    }
  }
};
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
