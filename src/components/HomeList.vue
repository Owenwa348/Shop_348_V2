<script setup>
import{ ref }from "vue"
const travelList = ref([
                      {name:'Mo-Mo-Paradise', adult:659,child:329,
                      img: "https://img.wongnai.com/p/400x0/2021/12/02/0d42a3543e0f465a9288f50bae220739.jpg", },
                      {name:'AKIYOSHI', adult: 599,child: 299,
                      img: "https://f.ptcdn.info/686/063/000/pqlwuv44lDNL45Kw83A-o.jpg", },
                      {name:'Kagonoya', adult: 549,child: 275,
                      img: "https://www.ryoiireview.com/upload/editor_review/202112/1638852621_db795edc4d74f3f820e8f69d68b718e2.jpg", },
                      {name:'tajimaya shabu', adult: 530,child: 265 ,
                      img: "https://hello2day.com/wp-content/uploads/2019/02/tajimaya-thailand-central-world-isetan-1.jpg", },
                      {name:'masaru shabu & sushi buffet', adult: 690,child: 270 ,
                      img: "https://kiji.life/eats/wp-content/uploads/2020/01/masaru-shabu-fcm_0406-1024x682.jpg", },
                      {name:'shiroku shabu', adult: 389,child: 389 ,
                      img: "https://www.ryoiireview.com/upload/editor_review/201606/1466746327_5b53f0b203a2cfa94ce924ab9b910e7d.jpg", },
                    ])


</script>
<template>
<div class="album py-5 bg-body-tertiary">
    <div class="container">
      <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
        <div class="col" v-for="(item,index) in travelList" :key="index">
          <div class="card shadow-sm">
            <img class="bd-placeholder-img card-img-top" width="100%" height="225" role="img" :src="item.img" alt="รูปภาพของ {{ item.name }}" aria-label="รูปภาพของ {{ item.name }}" preserveAspectRatio="xMidYMid slice" focusable="false">
            <div class="card-body">
              <strong class="d-inline-block mb-2 text-primary-emphasis">ร้านที่ {{ index + 1 }}</strong>
              <h1 class="card-title">{{ item.name }}</h1>
              <div class="mb-1 text-body-secondary">ราคาสำหรับผู้ใหญ่: {{ item.adult }} บาท</div>
              <div class="mb-1 text-body-secondary">ราคาสำหรับเด็ก: {{ item.child }} บาท</div>
              <p>กดเพื่อจองร้านที่ {{ index + 1 }}</p>
              <div class="d-flex justify-content-between align-items-center">
                <div class="btn-group">
                  <RouterLink to="NextList" type="button" class="btn btn-sm btn-outline-secondary">จองโต็ะ</RouterLink>
                </div>
                <small class="text-body-secondary"></small>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>