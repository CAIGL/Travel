<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
    </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'

export default {
  name: 'Home',
  components: {
    HomeHeader, /* es6 键名键值相同 HomeHeader == HomeHeader："HomeHeader" */
    HomeSwiper
  }
}
</script>

<style>

</style>
