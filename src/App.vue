<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Tolist v-for="(item,index) in list" :key='index' :message='item'></Tolist>
    <Aeader></Aeader>
     <bread></bread>
     <card></card>
     <caurse></caurse>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Tolist from './components/tolist'
import Aeader from './components/Aeader'
import bread from './components/bread'
import card from './components/Card'
import caurse from './components/caurse'
export default {
  name: 'app',
  data(){
    return {
      list:[
        {name:'a'},
        {name:'b'},
        {name:'c'}
      ]
    }
  },
  components: {
    HelloWorld,Tolist,Aeader, bread ,card,caurse
  },
 
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
