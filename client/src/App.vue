<template>
  <div id="app">
    <header class="d-flex mt-3 mb-4">
      <router-link class="ml-4" :to="{name:'yaara'}">לדף של יערה</router-link>
      <router-link class="ml-4" :to="{name:'home'}">בית</router-link>
      <!-- <router-link  class="ml-4" :to="{name:'createReport'}">צור דיווח רכב</router-link> -->
      <router-link  class="ml-4" to="/rrrrr">הרשמה</router-link>

      
    </header>
    <router-view />
    <ovarlayManager/>
  </div>
</template>

<script>
import ovarlayManager from './components/overlayManager.vue'
import homePage from './components/Home.vue'

export default {
  name: 'app',
  components: {
    homePage, ovarlayManager
  },
}
</script>

<style>
@import "./assets/styles/index.scss";

#app {
  text-align: right;
  direction: rtl;
}
</style>
