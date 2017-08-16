<template>
  <div class="menu">
    <div class="user">
      <div>
        张三
      </div>
    </div>

    <div class="theme">
      <router-link class="link icon-paragraph-justify">全部</router-link>
    </div>

    <div class="about">
      <router-link class="link icon-info">关于</router-link>
    </div>

    <div class="msg" v-if="user.loginname">
      <router-link class="link icon-envelope">消息</router-link>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  export default {
    data() {
      return {
        msgcount: 0,
        user: {}
      }
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .menu
    position: fixed
    width: 140px
    top:0
    bottom: 0
    left: -200px
    padding: 30px
    background:#7e8c8d
    transition: 0.3s
    z-index:999
</style>
