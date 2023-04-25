<template>
  <div class="footer">
    <button class="button footer__button">
      Go <span>-</span> Surf
      <img src="@/assets/svg/ShapeLeft.svg" alt="">
    </button>
    <p>© FMR 2023. All Rights Reserved.</p>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.footer {
  text-align: center;
  display: grid;
  justify-content: center;
  margin-top: 7rem;
  &__button {
    margin-bottom: 1rem;
    &::before {
      content: '';
      right: 1.4rem !important;
      width: 11rem !important;
    }
  }
  p{
    margin-bottom: 2rem;
  }
}
</style>
