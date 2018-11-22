<template>
    <div>
        <home-header></home-header>
    </div>
</template>

<script>
import HomeHeader from './components/Header'
export default {
  name: 'Home',
  components: {
    HomeHeader /* es6 键名键值相同 HomeHeader == HomeHeader："HomeHeader" */
  }
}
</script>

<style>

</style>
