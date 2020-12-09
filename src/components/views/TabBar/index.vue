<template>
  <div class="tabbar">
    <div class="logo">
      <img alt="site-logo" src="@/assets/img/home/logo.png" @click="goHome" />
    </div>
    <div class="go-back" @click="goBack">
      &lt; 返回
    </div>
    <router-link :to="item.link" v-for="(item, index) in routeList" :key="index">
      <div :class="{title:item.image=='', action:currentIndex==index}" @click="goTo(index)">
        <div>
          <img :src="item.image" alt />
          {{ item.title }}
        </div>
      </div>
    </router-link>
  </div>
</template>
<script>
export default {
  name: "TabBar",
  components:{},
  data() {
    return {
      currentIndex: 0,
      routeList: [
        {
          link: "/vtuber", image: require("@/assets/img/tabbar/vtuber.svg"), title: "Vtuber"
        },
      ]
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
    goTo(index) {
      if(this.routeList[index].image == '') return
      this.currentIndex = index
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