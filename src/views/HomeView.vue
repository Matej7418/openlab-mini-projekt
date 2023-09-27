<template>
  <main>
    <TheWelcome />
    <SvgMap
    :map="map"
    view-box="0 0 25220 23850"
    :thin-border-on-zoom="true"
  />
  </main>
</template>

<script lang="js">
import TheWelcome from '../components/TheWelcome.vue'
import SvgMap from 'vue-simple-svg-map'
import map from '@/assets/map.js'

export default {
  name: 'HomeView',
  components: {TheWelcome, SvgMap},
  data () {
    return {
      map
    }
  }
}
</script>