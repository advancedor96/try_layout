<template>
  <div id="app">
    <header class="header">
      <div class="container">


        <div class="logo">Shoptime</div>
        <button class="menubar" @click="isShow = !isShow">≡</button>
        <ul :class="{ 'isShow' : isShow}">
          <li><a href="/" class="active">Home</a></li>
          <li><a href="/">Order</a></li>
          <li><a href="/">Product</a></li>
          <li class="login">
            Admin
          </li>
        </ul>


      </div>
    </header>
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  data(){
    return {
      isShow:true
    }
  }
}
</script>

<style>
#app {

}
</style>
