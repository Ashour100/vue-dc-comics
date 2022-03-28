<template>
  <div id="app" class="m-0">
    <IndexHeader/>
    <IndexContent/>
    <IndexFooter/>
  </div>
</template>

<script>
import IndexHeader from './components/header.vue';
import IndexContent from './components/Content.vue';
import IndexFooter from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexContent,
    IndexFooter,
  }
}
</script>

<style lang="scss">
@import "./assets/style.scss"; 
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
@import'~bootstrap/dist/css/bootstrap.css'
</style>
