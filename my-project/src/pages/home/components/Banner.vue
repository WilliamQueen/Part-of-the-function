<template>
  <swiper class="swiper" :options="swiperOption">
    <swiper-slide v-for="item of bannerList" :key="item.id">
      <img class="banner-img" :src="item.imgUrl"/>
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
    <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div>
  </swiper>
</template>

<script>
import image1 from '../../../assets/images/banner1.jpg'
import image2 from '../../../assets/images/banner2.jpg'
export default {
  name: 'HomeBanner',
  data () {
    return {
      swiperOption: {
        autoplay: true,
        loop: true
      },
      bannerList: [
        {id: '0001', imgUrl: image1},
        {id: '0002', imgUrl: image2}
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .swiper
    height: 0
    overflow: hidden
    padding-bottom: 39.6%
    margin: 0 15px
    .banner-img
      width: 100%
</style>
