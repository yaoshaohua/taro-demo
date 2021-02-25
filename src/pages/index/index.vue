<template>
  <view class="index">
    <text>{{ msg }}</text>
    <swiper
      class="test-h"
      indicator-color="#999"
      indicator-active-color="#333"
      vertical
      circular
      indicator-dots
      autoplay
    >
      <swiper-item>
        <view class="demo-text-1">1</view>
      </swiper-item>
      <swiper-item>
        <view class="demo-text-2">2</view>
      </swiper-item>
      <swiper-item>
        <view class="demo-text-3">3</view>
      </swiper-item>
    </swiper>
  </view>
</template>

<script>
import { ref } from "vue";
import "./index.less";

export default {
  setup() {
    const msg = ref("Hello ysh");
    return {
      msg,
    };
  },
};
</script>
<style>
.flex-wrp {
  display: flex;
}
.flex-wrp-column {
  flex-direction: column;
}
.flex-wrp-row {
  flex-direction: row;
  padding: 20px;
  background: #f1f1f1;
}
.flex-item {
  width: 180px;
  height: 90px;
}
.demo-text-1 {
  background: #ccc;
}
.demo-text-2 {
  background: #999;
}
.demo-text-3 {
  background: #666;
}
.hover {
  background: #000;
}
</style>
