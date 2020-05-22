<template>
  <div class="page-home">
    <!--首页的头部 begin-->
    <header class="index-header">
      <a href="mine.html?cpid=0">
        <div class="header-user">
          <div class="user-btn"></div>
        </div>
      </a>
      <div class="header-logo"></div>
      <a href="search.html?cpid=0">
        <div class="header-search"></div>
      </a>
    </header>
    <!--首页头部 end-->
    <Swiper :autoplay="1000" @change="onChange" class="my-swiper">
    <SwiperItem><img src="../../assets/icon/lunbo.png" /></SwiperItem>
    <SwiperItem><img src="../../assets/icon/lunbo2.png" /></SwiperItem>
    <SwiperItem><img src="../../assets/icon/lunbo3.png" /></SwiperItem>
    <SwiperItem><img src="../../assets/icon/lunbo4.png" /></SwiperItem>
    <SwiperItem><img src="../../assets/icon/lunbo5.png" /></SwiperItem>
    </Swiper>
  </div>
</template>

<script>
/* import Swiper from '@/components/Swiper/Swiper.vue'
import SwiperItem from '@/components/Swiper/SwiperItem.vue' */
import { Swiper, SwiperItem } from '@/components/Swiper'

export default {
  name: 'Home',
  components: {
    Swiper,
    SwiperItem
  },

  methods: {
    onChange (index) {
      // console.log('你好', index)
    }
  }
}
</script>
<style lang="scss" scoped>
.page-home {
  display: flex;
  flex-direction: column;
  height: 100%;
  .index-header {
    display: flex;
    height: 44px;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    box-sizing: border-box;
    .user-btn {
      width: 25px;
      height: 25px;
      background: url("../../assets/icon/user-btn.png") no-repeat;
      background-size: 100%;
    }
    .header-logo {
      width: 92px;
      height: 28px;
      background: url("../../assets/icon/header-logo.png") no-repeat;
      background-size: 100%;
    }
    .header-search {
      width: 25px;
      height: 25px;
      background: url("../../assets/icon/search.png") no-repeat;
      background-size: 100%;
    }
  }
  .my-swiper img {
    width: 100%;
  }
}
</style>
