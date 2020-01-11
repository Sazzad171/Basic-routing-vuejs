<template>
  <div id="app">
    <router-link to="/helloworld">Home</router-link>
    <router-view></router-view>
  </div>
</template>


<script>
import Router from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'

const routes = [
  { path: '/helloworld', component: HelloWorld }
]

const router = new Router({
routes: routes,
mode: 'history'
})

export default {
  name: 'app',
  router
}
</script>

<style>

</style>
