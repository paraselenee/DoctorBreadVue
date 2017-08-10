<template>
  <div id="app">
    <firstcomponent></firstcomponent>  
    <p>{{message}}</p>
    <input v-model="message">
    <router-link :to="path" >点我</router-link>
    <!-- <router-link :to="{path: '/second'}" >点我</router-link> -->
  </div> 
</template>

<script>
import firstcomponent from './component/firstcomponent.vue'

export default {
  name: 'app',
  data () {
    return {
      message: 'Welcome to Your Vue.js App',
      path: '/second'
    }
  },
  components: { 
    firstcomponent
  }
}
// var app6 = new Vue({
//   el: '#app',
//   data:{
//     message: 'Hello Vue'
//   }
 
// })
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

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
