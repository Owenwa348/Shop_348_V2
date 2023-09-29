<script setup>
// import { computed } from 'vue';
// import ToCartList from '../router/bridgeA';

// function calculateTotalItems(ToCartList){
//   return ToCartList.reduce((total,item) => total + item.quantity,0);
// }
// const TotalItem = computed (() => calculateTotalItems(ToCartList.value));
</script>
<template>

<div class="container">
  <header class="border-bottom lh-1 py-3">
    <div class="row flex-nowrap justify-content-between align-items-center">
      <div class="col-4 pt-1">
        <img src="https://i0.wp.com/marketeeronline.co/wp-content/uploads/2015/06/Tseng_BaconAndEgg.jpg?resize=616%2C616&ssl=1" alt="Logo" width="50" height="50" class="d-inline-block align-text-top">
      </div>
      <div class="col-4 text-center">
        <header class="blog-header-logo text-body-emphasis text-decoration-none" href="#">God Of Food</header>
      </div>
      <div class="col-4 d-flex justify-content-end align-items-center">
        <a class="link-secondary" href="#" aria-label="Search">
          <!-- <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="mx-3" role="img" viewBox="0 0 24 24"><title>Search</title><circle cx="10.5" cy="10.5" r="7.5"/><path d="M21 21l-5.2-5.2"/></svg> -->
        </a>
        <!-- <button class="btn btn-sm btn-outline-secondary" @click="ToCartList" type="submit">บิลจองโต็ะ</button> -->
      </div>
    </div>
  </header>
</div>

</template>