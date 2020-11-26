<template>
  <div class="tabbar">
    <div class="logo">
      <img alt="site-logo" src="@/assets/img/logo.png" @click="goHome" />
    </div>
    <div class="go-back" @click="goBack">
      &lt; 返回
    </div>
    <router-link :to="item.link" v-for="(item, index) in routeList" :key="index">
    
    </router-link>
  </div>
</template>
<script>
export default {
  name: "TabBar",
  components:{},
  data() {
    return {
      routeList: []
    }
  },
  methods: {
    goHome() {
      if (this.$route.path != '/') {
        this.$router.push('/')
      }
    },
    goBack() {
      this.$router.go(-1)
    },
  },
}
</script>
<style lang="stylus">
.tabbar
  .logo
    display inline
    float left
    img 
      cursor pointer
      height 40px
      width 40px 
  .go-back
    display inline
    float left
    cursor pointer
</style>