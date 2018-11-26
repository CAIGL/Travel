<template>
    <div class="wrapper">
      <swiper :options="swiperOption">
        <!-- slides -->
        <swiper-slide v-for="item of swiperList" :key="item.id">
          <img class="swiper-img" :src="item.imgUrl" alt="">
        </swiper-slide>
        <!-- Optional controls -->
        <div class="swiper-pagination" slot="pagination"></div>
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
        loop: true,
        autoplay: 3000
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/8c/b9e86352f9aa5f02.jpg_750x200_2fe2875f.jpg'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/7c/8e5c4ab8ee8b7402.jpg_750x200_dd7a38dd.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper // 自动撑开高度
    overflow: hidden
    width: 100%
    height 0
    padding-bottom: 26.66%
    background: #eee
    .swiper-img
      width: 100%
    >>>.swiper-pagination-bullet-active // >>>进行样式穿透
      background: #fff
</style>
