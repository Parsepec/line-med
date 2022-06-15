<template>
  <swiper
    :slides-per-view="1"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide><div class="relative"><img :src="banner2" class="w-full h-screen" alt=""></div> </swiper-slide>
    <swiper-slide>Slide 2</swiper-slide>
    <swiper-slide>Slide 3</swiper-slide>
    ...
  </swiper>
</template>
<script setup lang="ts">
// Import Swiper Vue.js components
import aboutimg from '../images/linemed-about.jpg';
import banner from '../images/linemed-banner.jpg'
import banner2 from '../images/linemed-banner2.jpeg'
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css/bundle";

const onSwiper = (swiper) => {
  console.log(swiper);
};
const onSlideChange = () => {
  console.log("slide change");
};
</script>
