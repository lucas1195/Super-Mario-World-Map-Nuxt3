<template>
  <v-container class="body">
    <h1>Super Mario World Google Map</h1>
    <GoogleMap
      api-key="AIzaSyAW6yl01KyRZ2okcdLHY7ELIY8S_mEL24o"
      mapId="911da5329f148e36"
      style="width: 100%; height: 500px"
      :center="center"
      :zoom="16"
    >
      <Marker :options="markerOptions" />
    </GoogleMap>
  </v-container>
</template>

<script setup lang="ts">
/***-------IMPORTS-------***/
import { GoogleMap, Marker } from "vue3-google-map";
/***-------IMPORTS-------***/

/***-------VARIAVEIS-------***/
const center = { lat: 34.667996827004515, lng: 135.4303391005573 };
const markerOptions = { position: center, label: "L", title: "LADY LIBERTY" };
/***-------VARIAVEIS-------***/

/***-------FUNCOES-------***/

/***-------FUNCOES-------***/
</script>

<style>
*,
*::before,
*::after {
  box-sizing: inherit;
}

.body {
  margin: 0;
  padding: 0;
  background-color: black;
  height: 100vh;
}

h1 {
  font-family: "Press Start 2P", system-ui;
  color: white;
  font-weight: 400;
  font-style: normal;
}
</style>
