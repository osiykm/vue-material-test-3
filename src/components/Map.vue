<template>
  <MglMap
    :accessToken="accessToken"
    :mapStyle.sync="mapStyle"
    class="map"
  >
    <MglNavigationControl position="top-right"></MglNavigationControl>
    <MglGeolocateControl position="top-right"></MglGeolocateControl>
  </MglMap>
</template>

<script>
import Mapbox from 'mapbox-gl';
import { MglMap } from 'vue-mapbox';

export default {
  name: 'Map',
  components: {
    MglMap,
  },
  data() {
    return {
      accessToken: 'pk.eyJ1IjoiYWthaGl0byIsImEiOiItNzVLd0wwIn0.KONunqOpXmyebciuSMz0Hg', // your access token. Needed if you using Mapbox maps
      mapStyle: 'mapbox://styles/akahito/cjw3gnisa0z9r1cqnigk8meff', // your map style
    };
  },
  created() {
    // We need to set mapbox-gl library here in order to use it in template
    this.mapbox = Mapbox;
  },
};
</script>

<style scoped>
  .map {
    width: 100%;
    height: 500px;
    position: center;
  }

</style>
