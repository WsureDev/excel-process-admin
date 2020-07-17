<template>
  <div id="app">

<!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <BaseCard>
      <img src="./assets/logo.png" alt="">
      <div>
        <el-button>el-button</el-button>
      </div>
      <p>
        If Element is successfully added to this project, you'll see an
        <code v-text="'<el-button>'"></code>
        below
      </p>
    </BaseCard>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import BaseCard from "./components/BaseCard";

export default {
  name: 'app',
  components: {
    // HelloWorld,
    BaseCard
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
