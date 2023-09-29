<script setup>
import { RouterView } from 'vue-router'


</script>

<template>
  <div class="container">
    <HeaderList title ="God Of Food"></HeaderList>
    
    <div class="main">
      <RouterView />
    </div>
    <header>
      <nav></nav>
    </header>
    <div class="slide"></div>
  </div>
  <div class="footer"></div>
</template>

<style scoped>

</style>

