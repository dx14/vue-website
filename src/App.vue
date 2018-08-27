<template>
  <div>
    <router-view/>
  </div>
</template>

<script>
import Home from './components/Home.vue'
import About from './components/About.vue'
import Work from './components/Work.vue'
export default {
  name: 'app',
  data() {
    return {
      currentPage: 'home'
    }
  },
  components: {
    Home,
    About,
    Work
  }
}
</script>

<style>
body {
  background: url("./assets/background.jpg") no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-color: white;
}
</style>
