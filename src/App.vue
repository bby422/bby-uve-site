
<template>
  <div id="app">
    <img src="./assets/logo.png">
    {{msg}}
    <!-- 这里可以控制变量输入 -->
    <input v-model="parentRel" />
    <!-- 这里绑定的parentRel是在data中的Rel -->
    <cbutton href="http://www.baidu.com" title="哈哈" text="点呀" v-bind:rel="parentRel" />
    <router-view/>
  </div>
</template>

<script>
import cbutton from './components/CButton'
export default {
  name: 'app',
  data () {
    return {
      msg: '你个傻逼孩子',
      parentRel: '要有'
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
