<template>
<div class="header">
  <div class="header-left">
    <img src="../../../assets/images/logo.png" alt="" />
  </div>
  <div class="header-logo">
    <img src="../../../assets/images/ycTitle.png" alt="" />
  </div>
  <div class="header-city-list">
    <span class="change-city">[切换影城]</span>
  </div>
  <div class="header-right">
    <span class="iconfont"> &#xe608; </span>
  </div>
</div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
.header
  display: flex;
  height: .72rem;
  background: url(../../../assets/images/bg.gif) repeat;
  justify-content:  space-around;
  align-items: center;
  .header-left
    width: 0.6rem;
    float: left;
    img
     width: 0.6rem;
     height: 0.45rem;
  .header-logo
    width: 1.6rem
    img
      width: 1.60rem;
      height: 27px;
  .header-city-list
    .change-city
      color: #fffe00;
  .header-right
    float: right;
</style>
