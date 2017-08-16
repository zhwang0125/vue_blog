<template>
  <div>
    <v-header @menuShow="showMenu=true"></v-header>
    <v-menu v-bind:style="{left:showMenu?0:'-200px'}" @menuHidden="showMenu=false"></v-menu>
    <div class="list-body">111</div>
  </div>
</template>

<script type="text/ecmascript-6">
  import vHeader from '../header/header.vue'
  import vMenu from '../menu/menu.vue'

  export default {
    data() {
      return {
        showMenu: false
      }
    },
    components: {
      vHeader,
      vMenu
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .list-body
    margin-top 50px
</style>
