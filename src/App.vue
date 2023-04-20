<template>
  <t-header />
  <main class="main">
    <router-view/>
  </main>
  <t-footer />
</template>

<script>
import TFooter from './components/t-footer.vue'
import THeader from './components/t-header.vue'

export default {
  components: {
    THeader,
    TFooter
  }
}
</script>
