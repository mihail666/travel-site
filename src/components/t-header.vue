<template>
  <div class="header">
    <aside class="asideBar">
      <div class="aside-logo">
        <div>GO <span class="aside-logo-span"> - </span> SURF</div>
      </div>
      <div class="aside-menu menu">
        <div class="menu-group">
          <img class="menu-img" src="@/assets/svg/Surf.svg" alt="">
          <div class="menu-title">Surf</div>
        </div>
        <div class="menu-group">
          <img class="menu-img" src="@/assets/svg/Travel.svg" alt="">
          <div class="menu-title">Travel</div>
        </div>
        <div class="menu-group">
          <img class="menu-img" src="@/assets/svg/Camp.svg" alt="">
          <div class="menu-title">Sleep</div>
        </div>
        <div class="menu-group">
          <img class="menu-img" src="@/assets/svg/board.svg" alt="">
          <div class="menu-title">Shop</div>
        </div>
        <div class="menu-group">
          <img class="menu-icon" src="@/assets/svg/Search.svg" alt="">
        </div>
      </div>
      <div class="menu-date">
          <div class="menu-day">20</div>
          <div class="menu-date-info">06 | 2023</div>
        </div>
        <div class="menu-map">
          <img class="menu-icon" src="@/assets/svg/Shape.svg" alt="">
          <div class="menu-title">California</div>
        </div>
    </aside>

    <div class="parallax-bg"></div>
    <img class="map-bg" src="@/assets/imges/Map.png" alt="">

    <swiper
    :thumbs="{ swiper: thumbsSwiper}"
    :style="{
      '--swiper-navigation-color': '#fff',
      '--swiper-pagination-color': '#fff',
    }"
    :speed="600"
    :parallax="true"
    :pagination="{
      clickable: true,
    }"
    :navigation="true"
    :modules="modules"
    class="mySwiper"
  >
      <swiper-slide>
        <div class="swiper-slide__map map-mark-1">North Shore | Malibu, CA</div>
        <div class="swiper-slide__container container">
          <div class="subtitle-left" data-swiper-parallax="-200">Surf</div>
          <div class="title swiper-slide__title" data-swiper-parallax="-300">North Shore</div>
          <div class="subtitle-left" data-swiper-parallax="-200">ConSurfdition</div>
          <div class="text swiper-slide__text" data-swiper-parallax="-100">Radical</div>
          <a href="#" class="slider_btn">
            <img src="@/assets/svg/ShapeLeft.svg" alt="">
          </a>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="swiper-slide__map map-mark-2">South Shore | Malibu, CA</div>
        <div class="swiper-slide__container">
          <div class="subtitle-left" data-swiper-parallax="-200">Surf</div>
          <div class="title swiper-slide__title" data-swiper-parallax="-300">South Shore</div>
          <div class="subtitle-left" data-swiper-parallax="-200">ConSurfdition</div>
          <div class="text swiper-slide__text" data-swiper-parallax="-100">Radical</div>
          <a href="#" class="slider_btn">
            <img src="@/assets/svg/ShapeLeft.svg" alt="">
          </a>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="swiper-slide__map map-mark-3">West Shore | Malibu, CA</div>
        <div class="swiper-slide__container container">
          <div class="subtitle-left" data-swiper-parallax="-200">Surf</div>
          <div class="title swiper-slide__title" data-swiper-parallax="-300">West Shore</div>
          <div class="subtitle-left" data-swiper-parallax="-200">ConSurfdition</div>
          <div class="text swiper-slide__text" data-swiper-parallax="-100">Radical</div>
          <a href="#" class="slider_btn">
            <img src="@/assets/svg/ShapeLeft.svg" alt="">
          </a>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="swiper-slide__map map-mark-4">East Shore | Malibu, CA</div>
        <div class="swiper-slide__container container">
          <div class="subtitle-left" data-swiper-parallax="-200">Surf</div>
          <div class="title swiper-slide__title" data-swiper-parallax="-300">East Shore</div>
          <div class="subtitle-left" data-swiper-parallax="-200">ConSurfdition</div>
          <div class="text swiper-slide__text" data-swiper-parallax="-100">Radical</div>
          <a href="#" class="slider_btn">
            <img src="@/assets/svg/ShapeLeft.svg" alt="">
          </a>
        </div>
      </swiper-slide>
    </swiper>

    <div class="header-nav">
      <div class="header-button">
        <img src="@/assets/svg/DownArrows.svg" alt="">
      </div>

      <swiper
        @swiper="setThumbsSwiper"
        :spaceBetween="20"
        :slidesPerView="4"
        :freeMode="true"
        :watchSlidesProgress="true"
        :modules="modules"
        class="mySwiper__nav nav"
      >
        <swiper-slide class="nav__content">
          <div class="nav__item-data">
            <div class="nav__item-title" data-swiper-parallax="-100">01</div>
            <div class="nav__item-subtitle" data-swiper-parallax="-100">North Shore</div>
          </div>
        </swiper-slide>
        <swiper-slide class="nav__content">
          <div class="nav__item-data">
            <div class="nav__item-title" data-swiper-parallax="-100">02</div>
            <div class="nav__item-subtitle" data-swiper-parallax="-100">South Shore</div>
          </div>
        </swiper-slide>
        <swiper-slide class="nav__content">
          <div class="nav__item-data">
            <div class="nav__item-title" data-swiper-parallax="-100">03</div>
            <div class="nav__item-subtitle" data-swiper-parallax="-100">West Shore </div>
          </div>
        </swiper-slide>
        <swiper-slide class="nav__content">
          <div class="nav__item-data">
            <div class="nav__item-title" data-swiper-parallax="-100">04</div>
            <div class="nav__item-subtitle" data-swiper-parallax="-100">East Shore</div>
          </div>
        </swiper-slide>
      </swiper>
    </div>

  </div>
</template>
<script>

import { Swiper, SwiperSlide } from 'swiper/vue'

import 'swiper/css'
import 'swiper/css/pagination'
import 'swiper/css/navigation'

// import required modules
import { Parallax, Navigation, Thumbs } from 'swiper'
import { ref } from 'vue'
export default {
  components: {
    Swiper,
    SwiperSlide
  },
  setup () {
    const thumbsSwiper = ref(null)
    const setThumbsSwiper = (swiper) => {
      thumbsSwiper.value = swiper
    }
    return {
      modules: [Parallax, Navigation, Thumbs],
      setThumbsSwiper,
      thumbsSwiper
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/styles/variables.scss';
.header {
  position: relative;
  display: grid;
}
.header-nav {
  position: absolute;
  width: calc(100% - 200px);
  height: 100vh;
}
.header-button {
  position: absolute;
  left: 15rem;
  bottom: 1rem;
  animation: move 1.5s infinite;
  z-index: $z-tooltip;
}
@keyframes move {
  0% {
    bottom: 1rem;
  }
  50% {
    bottom: 2rem;
  }
}
.asideBar {
  position: absolute;
  left: 0;
  min-height: 100vh;
  width: 200px;
  border-right: 2px solid $border-color-alt;
  z-index: $z-fixed;
  display: grid;
  flex-wrap: wrap;
  grid-template-rows: max-content;
  overflow: hidden;
}
.aside-logo {
  width: 198px;
  position: relative;
  font-size: 4rem;
  font-weight: $font-bold;
  color: $white-color;
  writing-mode: vertical-lr;
  transform: rotate(180deg);
  margin-bottom: 5rem;
  margin-top: 2rem;
  display: flex;
  align-items: center;
  &::before {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    top: 38%;
    background-color: $first-color;
    z-index: -1;
  }
}
.aside-logo-span {
  position: relative;
  font-weight: $font-medium;
}
.aside-menu {
    display: grid;
    justify-content: center;
    text-align: center;
    row-gap: 1rem;
    justify-self: center;
    .menu-img {
      width: 55px;
      height: 45px;
    }
    .menu-icon {
      width: 24px;
      height: 24px;
    }
  }
.menu-date {
  display: grid;
  justify-content: center;
}
.menu-date-info  {
  position: absolute;
  left: 34%;
  bottom: 4.8rem;
}
.menu-day {
  font-size: $h1-font-size;
  font-weight: $font-bold;
}
.menu-map {
  margin: 0 auto;
  width: 90px;
  display: flex;
  justify-content: space-around;
  img {
    width: 11px;
    height: 14px;
  }
}

.mySwiper {
  margin-left: 200px;
  margin-right: auto;
  position: relative;
  width: calc(100% - 200px);
  height: 100vh;
}

.swiper-slide {
  position: relative;
  color: #fff;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  text-align: right;
  &__container {
    position: absolute;
    bottom: 7rem;
    right: 5rem;
    text-align: right;
  }

  &__title {
    margin: 0rem 0 2rem 0;
  }

  &__text {
    margin: 1rem 0;
  }

  &__map {
    position: absolute;
  }
}
.map-mark-1 {
  top: 10.9rem;
  right: 44%;
}
.map-mark-2 {
  top: 15.5rem;
  right: 30%;
}
.map-mark-3 {
  top: 17.5rem;
  right: 24%;
}
.map-mark-4 {
  top: 23rem;
  right: 20%;
}
.parallax-bg {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-image: url('@/assets/imges/headerBG.jpg');
  -webkit-background-size: cover;
  background-size: cover;
  background-position: center;
}
.map-bg {
  position: absolute;
  right: 0;
  top: 0;
  width: 1060px;
  height: 40%;
}

.swiper-button-prev,
.swiper-button-next {
  width: 30px;
  height: 21px;
  position: absolute;
  background-image: url('@/assets/svg/ShapeLeft.svg');
  background-repeat: no-repeat;
  left: auto;
  right: 5rem;
  top: 5rem;
  &::after {
    content: "";
  }
}
.swiper-button-prev {
  right: 8rem;
  rotate: 180deg;
}
.slider_btn {
  display: inline-block;
  margin-top: 1rem;
}

.nav {
  position: absolute;
  height: 4rem;
  width: 600px;
  right: -7.5rem;
  z-index: $z-fixed;
  bottom: 0rem;
  cursor: pointer;
  &__content {
    border-top: 4px solid $text-color-light;
    &:focus {
      border-top: 4px solid $first-color;
    }
  }
  &__item-data{
    color: $text-color-light;
    margin-top: .5rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  &__item-title {
    font-size: $h2-font-size;
    font-weight: $font-bold;
  }
  &__item-subtitle {
    font-size: $h3-font-size;
  }
}
.swiper-slide-thumb-active {
  border-top: 4px solid $first-color;
}
.swiper-slide-thumb-active .nav__item-data{
  color: $white-color;
}
.swiper-slide-active .nav__item-data{
  color: $white-color;
}
// .swiper-pagination {
//   right: 0;
// }
// .swiper-pagination-bullet {
//     border-radius: 0;
//     width: 200px;
//     height: 4px;
//     background: $text-color-light;
//     &::after{
//       content: '01';
//     }
// }

</style>
