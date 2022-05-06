<template>
  <div>
    <div class="swiper_wrap">
      <div class="swiper_left">
        <div
          class="swiper_left_item"
          v-for="(item, index) in list"
          :key="index"
        >
          <div class="swiper_left_item_text">{{ item }}</div>
          <div class="swiper_left_item_icon iconfont icon-dayuhao"></div>
        </div>
      </div>
      <div class="swiper_right">
        <el-carousel height="470px">
          <el-carousel-item v-for="item in 4" :key="item">
            <h3 class="small">{{ item }}</h3>
          </el-carousel-item>
        </el-carousel>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: [
        "手机",
        "电视",
        "笔记本 平板",
        "家电",
        "出行 穿戴",
        "智能 路由器",
        "电源 配件",
        "健康 儿童",
        "耳机 音响",
        "生活 箱包",
      ],
    };
  },
};
</script>

<style>
.swiper_wrap {
  display: flex;
  /* justify-content: space-between; */
}
.swiper_left {
  padding: 10px 0;
  margin: 0 0 0 166px;
  height: 450px;
  width: 180px;
  background: #959997;
  color: #fff;
}
.swiper_left_item {
  display: flex;
  justify-content: space-between;
  /* flex: 2; */
  padding: 12px 13px;
}
.swiper_left_item:hover {
    background: #ff6700;
}
.swiper_right {
  flex: 2;
  padding: 0 214px 0 0;
  /* background: pink; */
  /* float: right; */
}
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 150px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>
