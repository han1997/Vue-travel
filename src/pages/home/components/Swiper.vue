<template>
<!-- ref="mySwiper" @someSwiperEvent="callback" -->
  <div class="wraper">
    <swiper :options="swiperOption" >
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img width="100%" height="100px" :src="item.url">
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '0001',
        url: '//imgs.qunarzz.com/p/tts1/1508/f5/d39a001a272e3c.jpg_r_480x320x90_ab6add13.jpg'
      }, {
        id: '0002',
        url: '//imgs.qunarzz.com/p/tts0/1807/a0/9afd8e22985e7802.jpg_r_480x320x90_adf1bbe1.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wraper >>> .swiper-pagination-bullet-active
    background #ffffff
  .wraper
  // 此设置使swiper固定大小，下面的内容不会变换位置
    overflow hidden
    width 100%
    height 0
    padding-bottom 31.25%
</style>
