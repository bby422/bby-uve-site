
<template>
  <div id="app">
    <img src="./assets/logo.png">
    {{msg}}
    <cbutton href="http://www.baidu.com" title="哈哈" text="点呀" />
    <router-view/>
  </div>
</template>

<script>
import cbutton from './components/CButton'
export default {
  name: 'app',
  data () {
    return {
      msg: '你个傻逼孩子'
    }
  },
  components: {
    cbutton
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
