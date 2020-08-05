<template>
  <view>
    <view class="swiperWrap">
      <!-- 轮播组件 -->
      <myswiper></myswiper>
    </view>
    <view>
      <!-- 菜单 -->
      <view class="navContent">
        <view class="mynav">
          <view class="navitem">
            <img class="navImg" src="/static/images/1.png" alt />
            急救指南
          </view>
          <view class="navitem">
            <img class="navImg" src="/static/images/2.png" alt />
            急救动态
          </view>
          <view class="navitem">
            <img class="navImg" src="/static/images/3.png" alt />
            服务网点
          </view>
        </view>
        <!-- 第二行菜单 -->
        <view class="mynav">
          <view class="navitem">
            <img class="navImg" src="/static/images/4.png" alt />
            志愿者报名
          </view>
          <view class="navitem">
            <img class="navImg" src="/static/images/5.png" alt />
            急救视频
          </view>
          <view class="navitem">
            <img class="navImg" src="/static/images/6.png" alt />
            关于我们
          </view>
        </view>
      </view>
      <!-- 救援组件 -->
      <help></help>

      <!-- 新闻条 -->
      <news></news>
    </view>
  </view>
</template>

<script>
import help from "./help.vue";
import news from "./news.vue";
import myswiper from "./myswiper";
export default {
  data() {
    return {
      background: ["red", "color2", "color3"],
      indicatorDots: true,
      autoplay: true,
      interval: 2000,
      duration: 500
    };
  },
  methods: {},
  components: {
    help,
    news,
    myswiper
  }
};
</script>

<style lang="scss" scoped>
.navContent{
	margin: 40rpx 0;
}

.mynav {
  display: flex;
}
.navitem {
  flex: 1;
  text-align: center;
  font-size: 0.8em;
  color:rgb(104, 98, 98);
  margin-top: 14rpx;
  
}
.navImg {
  height: 70rpx;
  width: 70rpx;
  display: block;
  margin: 0 auto;
  margin-top: 10rpx;
}
</style>
