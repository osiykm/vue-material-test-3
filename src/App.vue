<template>
  <div id="app">
    <link rel="stylesheet"
          href="//fonts.googleapis.com/css?family=Roboto:400,500,700,400italic|Material+Icons">
    <link
      href="https://api.tiles.mapbox.com/mapbox-gl-js/v0.53.0/mapbox-gl.css"
      rel="stylesheet"
    />
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/map">Map</router-link> |
      <router-link to="/api">Api</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
}

</style>
