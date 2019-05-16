<template>
  <div id="app">
   <router-view></router-view>
   <!-- $route 当前路由； meta.showFooter 为true时显示FooterGuide组件 -->
    <FooterGuide v-if="$route.meta.showFooter"/>
  </div>
</template>

<script>
import FooterGuide from './components/FooterGuide/FooterGuide.vue'

export default {
  // name: 'App',
  // components: {
  //   HelloWorld
  // }
  components:{
    FooterGuide
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
.app
  width 100%
  height 100%
  background #f5f5f5
</style>
