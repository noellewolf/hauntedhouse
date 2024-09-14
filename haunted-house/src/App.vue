<script setup>
import HouseBackground from './components/HouseBackground.vue'
import House from './components/interactive/House.vue'
</script>

<template>
  <header>
    <title>Haunted House</title>
  </header>
  <body>
    <HouseBackground></HouseBackground>
    <House class="house-positioning"></House>
  </body>
</template>

<style scoped>
.house-positioning {
  position: absolute;
  color:black;
  top:10rem;
  left:18rem;
  width:50%;
  height:50%;
}
</style>
