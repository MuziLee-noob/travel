<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>输入城市/景点/游玩/主题</div>
    <router-link to="City">
      <div class="header-right">
        {{ this.$store.state.city }}<span class="iconfont arrow-icon">&#xe62d;</span>
      </div>
    </router-link>

  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  data () {
    return {

    }
  }
}
</script>
<!--1rem = html font-size = 50px-->
<style lang="stylus" scoped>
@import '~styles/varibles.styl'
  .header
    display: flex
    line-height: $headerHeight
    background: $bgColor
    color: #fff
    .header-left
      width: .64rem
      float: left
      .back-icon
        text-align: center
        font-size: .4rem
    .header-input
      flex: 1
      height: .64rem
      line-height: .64rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background: #fff
      border-radius: .1rem
      color: #ccc
    .header-right
      width: 1.24rem
      float: right
      text-align: center
      color: #fff
      .arrow-icon
        margin-left: .1rem
        font-size: .2rem
</style>
