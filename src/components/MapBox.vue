<template>
  <MapboxMap
    :center="mapCenter"
    :zoom="11"
    access-token="pk.eyJ1IjoiZmwwcjFhbjg0IiwiYSI6ImNseDU4dHkyYzFjdG8ya3M0cWt5NHYxeTQifQ.BOPdowVpzfpSn6qox_-nWw"
    map-style="mapbox://styles/mapbox/standard"
    style="height: 100vh; width: 100%"
  >
    <MapboxGeolocateControl />
  </MapboxMap>
</template>

<script lang="ts" setup>
import 'mapbox-gl/dist/mapbox-gl.css'
import { ref } from 'vue'
import { MapboxGeolocateControl, MapboxMap } from '@studiometa/vue-mapbox-gl'

const mapCenter = ref([6.958735655501745, 50.94179850699188])
</script>
