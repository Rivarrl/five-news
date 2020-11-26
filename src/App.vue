<template>
  <div id="app">
    <tab-bar></tab-bar>
  </div>
</template>
<script>
import TabBar from '@/components/views/TabBar/index'
export default {
  name:'App',
  components:{
    TabBar
  },
}
</script>
<style lang="stylus">
@import './assets/stylus/base.styl'
#app 
  width 100%
  height 100vh
  overflow hidden
  user-select none
  background #16181c
  color #fff
</style>
