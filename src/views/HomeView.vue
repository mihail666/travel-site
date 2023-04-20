<template>
  <div class="section-container bg">
    <section class="surf section">
      <div class="content-container grid">
        <div class="section-title">
          <span>
            SURF
            <h1>SURF</h1>
          </span>
        </div>

        <div class="surf__subtitle content-subtitle">
          <div class="subtitle">
            <img src="@/assets/icons/POI.png" alt="" class="surf__subtitle-icon">
            <img src="@/assets/icons/POI.png" alt="" class="surf__subtitle-icon-full">
            <h3 class="headline-left">Current location</h3>
            <h2 class="subtitle__head">California <span>|</span> USA</h2>
            <div class="surf__subtitle-text vetical-text">34.0501 N -118.2446 W</div>
          </div>
        </div>

        <div class="surf__map-img">
          <div class="surf__map">
            <div class="surf__map-poi" v-for="n in 9" :key="n">
              <div class="card">
                <div class="card__data">
                  <div class="card__title">
                    <h3>Airlie Beach</h3>
                    <img src="@/assets/svg/ShapeLeft.svg" alt="qwer">
                  </div>
                  <div class="card__subtitle">
                    Australia
                  </div>
                  <div class="card__content">
                    <div class="card__group">
                      <img src="@/assets/svg/Surf.svg" alt="">
                      <h3>9-13</h3>
                      <p>SURF(FT)</p>
                    </div>
                    <div class="card__group">
                      <img src="@/assets/svg/Surf.svg" alt="">
                      <h3>9-13</h3>
                      <p>SURF(FT)</p>
                    </div>
                    <div class="card__group">
                      <img src="@/assets/svg/Surf.svg" alt="">
                      <h3>9-13</h3>
                      <p>SURF(FT)</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

    </section>

    <section class="surfSwiper">
      <swiper class="surfSwiper__wrapper swiper-container"
        :mousewheel="true"
        :spaceBetween="0"
        :slidesPerView="4"
        :loop="true"
        :grabCursor="true"
        :modules="modules"
        :navigation="true"
      >
        <swiper-slide class="slide__content">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object1.png" alt="">
            <div class="slide__item-title">Malibu<br>Beach</div>
            <div class="slide__item-subtitle vetical-text">California <span>|</span> USA</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
        <swiper-slide class="slide__content">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object2.png" alt="">
            <div class="slide__item-title">Airlie<br>Beach</div>
            <div class="slide__item-subtitle vetical-text">Queensland <span>|</span> Australia</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
        <swiper-slide class="slide__content">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object3.png" alt="">
            <div class="slide__item-title">Cloud<br>Nine</div>
            <div class="slide__item-subtitle vetical-text">Siargao <span>|</span> Philippines</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
        <swiper-slide class="slide__content">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object4.png" alt="">
            <div class="slide__item-title">Vieux<br>Boucau</div>
            <div class="slide__item-subtitle vetical-text">Hossegor <span>|</span> France</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
        <swiper-slide class="slide__content">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object4.png" alt="">
            <div class="slide__item-title">Vieux<br>Boucau</div>
            <div class="slide__item-subtitle vetical-text">Hossegor <span>|</span> France</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
        <swiper-slide class="slide__content">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object3.png" alt="">
            <div class="slide__item-title">Cloud<br>Nine</div>
            <div class="slide__item-subtitle vetical-text">Siargao <span>|</span> Philippines</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
        <swiper-slide class="slide__content vetical-text">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object1.png" alt="">
            <div class="slide__item-title">Malibu<br>Beach</div>
            <div class="slide__item-subtitle">California <span>|</span> USA</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
        <swiper-slide class="slide__content">
          <div class="slide__item-data">
            <img class="slide__img" src="@/assets/imges/Object2.png" alt="">
            <div class="slide__item-title">Airlie<br>Beach</div>
            <div class="slide__item-subtitle vetical-text">Queensland <span>|</span> Australia</div>
            <button class="slide__item-button button">
              View<span>-</span>Surf
              <img src="@/assets/svg/ShapeLeft.svg" alt="">
            </button>
          </div>
        </swiper-slide>
      </swiper>
    </section>

    <section class="travel section">
      <div class="content-container grid">
        <div class="section-title">
          <span>
            Travel
            <h1>Travel</h1>
          </span>
        </div>
        <div class="sectionSwiper">
          <swiper class="sectionSwiper__wrapper"
            :spaceBetween="10"
            :slidesPerView="1"
            :loop="true"
            :grabCursor="true"
            :modules="modules"
            :navigation="true"
          >
            <swiper-slide class="slide__content">
              <div class="slide__item-data">
                <img class="slide__img" src="@/assets/imges/TravelImage.png" alt="">

                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-right">Airline</h3>
                    <h2 class="subtitle__head">Virgin Australia</h2>
                  </div>
                </div>
                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-left">Shore</h3>
                    <h2 class="subtitle__head">Airlie Beach <span>|</span> Australia</h2>
                  </div>
                </div>

                <img class="slide__img-bitmap" src="@/assets/imges/Bitmap.png" alt="">

                <div class="slide__group">
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Destination</h3>
                    <h2 class="data-title">Queensland <br> Australia</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Distance</h3>
                    <h2 class="data-title">7,065 Miles</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Travel Time</h3>
                    <h2 class="data-title">23 Hours <br> 5 Minutes</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Pricing</h3>
                    <div>
                      <h2 class="data-title">$ 1,976 USD</h2>
                      <p>Round Trip</p>
                    </div>
                  </div>
                </div>

                <button class="slide__button button">
                  Book <span>-</span> Flight
                  <img src="@/assets/svg/ShapeLeft.svg" alt="">
                </button>

                <img class="slide__img-cocktail" src="@/assets/imges/cocktail_PNG33.png" alt="">
              </div>
            </swiper-slide>

            <swiper-slide class="slide__content">
              <div class="slide__item-data">
                <img class="slide__img" src="@/assets/imges/TravelImage.png" alt="">

                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-right">Airline</h3>
                    <h2 class="subtitle__head">Virgin California</h2>
                  </div>
                </div>
                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-left">Shore</h3>
                    <h2 class="subtitle__head">Malibu Beach <span>|</span> California</h2>
                  </div>
                </div>

                <img class="slide__img-bitmap" src="@/assets/imges/Bitmap.png" alt="">

                <div class="slide__group">
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Destination</h3>
                    <h2 class="data-title">California <br> USA</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Distance</h3>
                    <h2 class="data-title">9,065 Miles</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Travel Time</h3>
                    <h2 class="data-title">24 Hours <br> 5 Minutes</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Pricing</h3>
                    <div>
                      <h2 class="data-title">$ 1,976 USD</h2>
                      <p>Round Trip</p>
                    </div>
                  </div>
                </div>

                <button class="slide__button button">
                  Book <span>-</span> Flight
                  <img src="@/assets/svg/ShapeLeft.svg" alt="">
                </button>

                <img class="slide__img-cocktail" src="@/assets/imges/cocktail_PNG33.png" alt="">
              </div>
            </swiper-slide>

            <swiper-slide class="slide__content">
              <div class="slide__item-data">
                <img class="slide__img" src="@/assets/imges/TravelImage.png" alt="">

                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-right">Airline</h3>
                    <h2 class="subtitle__head">Virgin Philippines</h2>
                  </div>
                </div>
                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-left">Shore</h3>
                    <h2 class="subtitle__head">Cloud Nine <span>|</span> Philippines</h2>
                  </div>
                </div>

                <img class="slide__img-bitmap" src="@/assets/imges/Bitmap.png" alt="">

                <div class="slide__group">
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Destination</h3>
                    <h2 class="data-title">Philippines <br> Siargao</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Distance</h3>
                    <h2 class="data-title">10,065 Miles</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Travel Time</h3>
                    <h2 class="data-title">34 Hours <br> 30 Minutes</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Pricing</h3>
                    <div>
                      <h2 class="data-title">$ 2,976 USD</h2>
                      <p>Round Trip</p>
                    </div>
                  </div>
                </div>

                <button class="slide__button button">
                  Book <span>-</span> Flight
                  <img src="@/assets/svg/ShapeLeft.svg" alt="">
                </button>

                <img class="slide__img-cocktail" src="@/assets/imges/cocktail_PNG33.png" alt="">
              </div>
            </swiper-slide>

            <swiper-slide class="slide__content">
              <div class="slide__item-data">
                <img class="slide__img" src="@/assets/imges/TravelImage.png" alt="">

                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-right">Airline</h3>
                    <h2 class="subtitle__head">Virgin Australia</h2>
                  </div>
                </div>
                <div class="slide__subtitle content-subtitle">
                  <div class="subtitle">
                    <h3 class="headline-left">Shore</h3>
                    <h2 class="subtitle__head">Vieux Boucau <span>|</span> France</h2>
                  </div>
                </div>

                <img class="slide__img-bitmap" src="@/assets/imges/Bitmap.png" alt="">

                <div class="slide__group">
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Destination</h3>
                    <h2 class="data-title">France <br> Hossegor</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Distance</h3>
                    <h2 class="data-title">8,065 Miles</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Travel Time</h3>
                    <h2 class="data-title">27 Hours <br> 10 Minutesa</h2>
                  </div>
                  <div class="slide__group-data">
                    <h3 class="data-subtitle vetical-text">Pricing</h3>
                    <div>
                      <h2 class="data-title">$ 2,176 USD</h2>
                      <p>Round Trip</p>
                    </div>
                  </div>
                </div>

                <button class="slide__button button">
                  Book <span>-</span> Flight
                  <img src="@/assets/svg/ShapeLeft.svg" alt="">
                </button>

                <img class="slide__img-cocktail" src="@/assets/imges/cocktail_PNG33.png" alt="">
              </div>
            </swiper-slide>
          </swiper>
        </div>
      </div>
    </section>
    <section class="sleep section">
      <div class="content-container grid">
        <div class="section-title">
          <span>
            Sleep
            <h1>Sleep</h1>
          </span>
        </div>

        <div class="sleep__subtitle content-subtitle">
          <div class="subtitle">
            <h3 class="headline-left">Current location</h3>
            <h2 class="subtitle__head">California <span>|</span> USA</h2>
          </div>
        </div>
      </div>
    </section>
    <section class="shop section">
      <div class="content-container grid">
        <div class="section-title">
          <span>
            Shop
            <h1>Shop</h1>
          </span>
        </div>

        <div class="shop__subtitle content-subtitle">
          <div class="subtitle">
            <h3 class="headline-left">Current location</h3>
            <h2 class="subtitle__head">California <span>|</span> USA</h2>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>

import { Swiper, SwiperSlide } from 'swiper/vue'

import 'swiper/css'
import 'swiper/css/pagination'
import 'swiper/css/navigation'

import { Pagination, Navigation, Mousewheel } from 'swiper'
export default {
  name: 'mainPage',
  components: {
    Swiper,
    SwiperSlide
  },
  setup () {
    return {
      modules: [Pagination, Navigation, Mousewheel]
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/styles/variables.scss';

.surf {
  position: relative;

  &__subtitle {
    position: relative;

    &-text {
      position: absolute;
      top: 22rem;
      right: 0rem;
      z-index: 1;
    }

    &-icon {
      position: absolute;
      right: -2rem;
      top: -8rem;
    }

    &-icon-full {
      position: absolute;
      right: -181px;
      top: -8rem;
      transform: scale(-1, 1);
    }
  }

  &__map {
    &-img {
      position: relative;
      top: 0rem;
      width: 100%;
      height: 650px;
      max-width: 1250px;
      background-repeat: no-repeat;
      background-image: url('../assets/imges/Map2.png');
      display: flex;
      justify-self: center;
      background-size: contain;
    }

    &-poi {
      position: absolute;
      width: 24px;
      height: 24px;
      border-radius: 50%;
      background-color: $first-color;
      box-shadow: 0px 0px 25px rgba(74, 246, 205, 0.84);
      left: 67rem;
      bottom: 6rem;
      animation: pulse 1.5s infinite;
      transition: .3s;

      @keyframes pulse {
        0% {
          box-shadow: 0px 0px 25px rgba(74, 246, 205, 0.84);
        }

        50% {
          box-shadow: 0px 0px 40px rgba(107, 255, 220, 1);
        }
      }

      &:hover {
        border-radius: 50% 0 50% 50%;
        transform: rotate(-45deg);
        z-index: 2;
      }

      &:hover .card {
        right: -13.5rem;
        top: -11rem;
        opacity: 1;
      }

      &:nth-child(2) {
        left: 0rem;
        top: 20.5rem;
      }

      &:nth-child(3) {
        left: 9rem;
        top: 18.5rem;
      }

      &:nth-child(4) {
        left: 20.5rem;
        top: 20rem;
      }

      &:nth-child(5) {
        left: 25rem;
        top: 31rem;
      }

      &:nth-child(6) {
        left: 33.5rem;
        top: 14rem;
      }

      &:nth-child(7) {
        left: 39.5rem;
        top: 34rem;
      }

      &:nth-child(8) {
        left: 50rem;
        top: 23.5rem;
      }

      &:nth-child(9) {
        left: 61rem;
        top: 20rem;
      }
    }
  }

  .card {
    opacity: 0;
    position: absolute;
    top: -100rem;
    right: 0rem;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 18rem;
    height: 13.5rem;
    border-radius: 6px;
    background: hsla(180, 3%, 6%, .7);
    transform: rotate(45deg);
    transition: .2s;

    &__title {
      position: relative;
      display: flex;
      justify-content: space-between;
      padding-bottom: 1rem;

      ::before {
        content: '';
        position: absolute;
        width: 5rem;
        height: 1px;
        left: 0;
        bottom: 0.5rem;
        background-color: $first-color;
      }
    }

    &__content {
      margin-top: 1.75rem;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      column-gap: 2rem;
    }
  }

}

.surfSwiper {
  position: relative;
  height: 950px;
  background: none;
  top: -5rem;

  &__wrapper {
    margin-left: auto;
    margin-right: auto;
    position: relative;

    &.swiper-button-prev {
      position: relative;
      top: -5rem;
    }
  }

  .slide__img {
    width: 450px;
    height: 750px;
    filter: brightness(75%);
  }

  .slide__content {
    position: relative;
    width: 400px !important;
    height: max-content;
    margin-top: 7rem;
    margin-right: -2rem;
    color: $white-color;
    filter: brightness(50%);
    transition: .3s;

    &:nth-child(2n+1) {
      margin-top: 10rem;
    }

    &:nth-child(3n) {
      margin-top: 13rem;
    }
  }

  .slide__item {
    &-data {
      height: 750px;
      transition: .3s;
    }

    &-title {
      position: absolute;
      top: 4.5rem;
      left: 3.5rem;
      font-size: $text-font-size;
      font-weight: $font-bold;
      line-height: 36px;
      text-align: left;
    }

    &-subtitle {
      position: absolute;
      top: 15rem;
      left: 3.5rem;
    }

    &-button {
      opacity: 1;
      position: absolute;
      left: 3rem;
      bottom: 0rem;
    }
  }

  .swiper-button-prev {
    right: 5rem;
  }

  .swiper-button-next {
    right: 2rem;
  }
}

</style>
