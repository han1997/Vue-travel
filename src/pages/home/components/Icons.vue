<template>
  <div class="icons">
    <div class="icon" v-for="item of iconlist" :key="item.id">
      <div class="icon-img">
        <img class="icon-img-content" :src="item.imgurl">
      </div>
      <p>热门景点</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      iconlist: [
        {
          id: '0001',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        },
        {
          id: '0002',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        },
        {
          id: '0003',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        },
        {
          id: '0004',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        },
        {
          id: '0005',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        },
        {
          id: '0006',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        },
        {
          id: '0007',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        },
        {
          id: '0008',
          imgurl:
            '//imgs.qunarzz.com/p/tts2/1506/f8/8bde875333634.jpg_r_480x320x90_e40a652a.jpg'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
.icons
  overflow: hidden
  height: 0
  padding-bottom: 50%
  background: green
  overflow hidden
  .icon
    position relative
    float: left
    height 0
    width: 25%
    padding-bottom: 25%
    .icon-img
      position absolute
      box-box-sizing border-box
      padding .1rem
      top 0
      left 0
      right 0
      bottom .44rem
      icon-img-content
        display block
        margin 0 auto
        height 100%
</style>
