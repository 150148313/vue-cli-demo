<template>
  <div id="app">
    <swiper ref="mySwiper" :options="swiperOption">
      <swiperSlide class="swiper-slide">Slide 1</swiperSlide>
      <swiperSlide class="swiper-slide">Slide 1</swiperSlide>
    </swiper>
  </div>
</template>

<script>
  import {Swiper, SwiperSlide} from 'vue-awesome-swiper'

  export default {
    name: 'App',
    components: {
      Swiper,
      SwiperSlide,
    },
    data(){
      return {
        swiperOption: {}
      }
    },
    methods: {
      swiper() {
        return this.$refs.mySwiper.$swiper
      }
    },
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
