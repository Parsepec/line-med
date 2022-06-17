<template>
  <swiper
    :slides-per-view="1"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide
      ><div class="relative flex">
        <div
          class="
            bg-gray-700
            opacity-70
            text-white
            absolute
            z-10
            rounded-2xl
            py-10
            inset-0
            px-10
            w-5/12
            mx-auto
            h-2/4
            my-auto
            flex
          "
        >
          <div
            class="flex flex-col opacity-100 text-center self-center mx-auto"
          >
            <div class="bg-white h-1 w-10 mb-4 rounded-md mx-auto"></div>
            <h1 class="font-header text-4xl">LinMed</h1>
            <p>Behavioral Health</p>
            <div class="inline-flex mt-4">
              <a
                href=""
                class="
                  bg-white
                  font-bold font-open
                  text-sm
                  mr-3
                  text-teal-700
                  px-4
                  py-2
                  rounded-2xl
                "
                >Contact Us</a
              >
              <a
                href=""
                class="
                  bg-white
                  font-bold font-open
                  text-sm
                  mr-3
                  text-teal-700
                  px-4
                  py-2
                  rounded-2xl
                "
                >Book an Appointment</a
              >
            </div>
          </div>
        </div>
        <img :src="banner2" class="w-full h-screen" alt="" />
      </div>
    </swiper-slide>
    <swiper-slide>
      
      <div class="relative flex">
        <div
          class="
            bg-gray-700
            opacity-70
            text-white
            absolute
            z-10
            rounded-2xl
            py-10
            inset-0
            px-10
            w-5/12
            mx-auto
            h-2/4
            my-auto
            flex
          "
        >
          <div
            class="flex flex-col opacity-100 text-center self-center mx-auto"
          >
            <div class="bg-white h-1 w-10 mb-4 rounded-md mx-auto"></div>
            <h1 class="font-header text-4xl">LinMed</h1>
            <p>Behavioral Health</p>
            <div class="inline-flex mt-4">
              <a
                href=""
                class="
                  bg-white
                  font-bold font-open
                  text-sm
                  mr-3
                  text-teal-700
                  px-4
                  py-2
                  rounded-2xl
                "
                >Contact Us</a
              >
              <a
                href=""
                class="
                  bg-white
                  font-bold font-open
                  text-sm
                  mr-3
                  text-teal-700
                  px-4
                  py-2
                  rounded-2xl
                "
                >Book an Appointment</a
              >
            </div>
          </div>
        </div>
        <img :src="banner" class="w-full h-screen" alt="" />
      </div>
    </swiper-slide>
    ...
  </swiper>
</template>
<script setup lang="ts">
// Import Swiper Vue.js components
import aboutimg from "../images/linemed-about.jpg";
import banner from "../images/linemed-banner.jpg";
import banner2 from "../images/linemed-banner2.jpeg";
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
