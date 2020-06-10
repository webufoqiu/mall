<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
// import axios from 'axios'
import jsonp from 'jsonp'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  mounted(){
    // let url1 = "https://easy-mock.com/mock/5ee0dade81099f496759c527/example/mock"
    // axios.get(url1).then(()=>{ })
    let url2='https://www.imooc.com/activity/servicetime';
    jsonp(url2,()=>{ })
  }
  // 跨域测试
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
