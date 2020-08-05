<template>
  <view>
    <view class="uni-padding-wrap">
      <view class="page-section swiper">
        <view class="page-section-spacing">
          <swiper
            class="swiper"
            :indicator-dots="indicatorDots"
            :autoplay="autoplay"
            :interval="interval"
            :duration="duration"
          >
            <swiper-item>
              <view class="swiper-item uni-bg-red">
                <img src="/static/images/header.png" alt />
              </view>
            </swiper-item>
            <swiper-item>
              <view class="swiper-item uni-bg-green">
                <img src="/static/images/header.png" alt />
              </view>
            </swiper-item>
            <swiper-item>
              <view class="swiper-item uni-bg-blue">
                <img src="/static/images/header.png" alt />
              </view>
            </swiper-item>
          </swiper>
        </view>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      background: ["color1", "color2", "color3"],
      indicatorDots: true,
      autoplay: true,
      interval: 2000,
      duration: 500
    };
  }
};
</script>

<style lang="scss" scoped>
.page-section .swiper{
  height: 240rpx;
  img{
    height: 240rpx;
    width: 100%;
  }
}
</style>

