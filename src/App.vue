<template>
  <t-header />
  <router-view/>
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
