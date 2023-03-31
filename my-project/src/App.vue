<template>
  <div>
    <img decoding="async" alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Hello Vue 3.0 + Vite" />
    <button @click="fun">增加年龄</button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import {myfunction} from '@/utils/test.js'
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  methods: {
    fun () {
      myfunction()
    }
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
