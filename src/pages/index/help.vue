<template>
  <view class="content">
    <view class="helpcontent">
      <view class="scannig">
        <img src="/static/images/7.png" alt />
        <br />
        <text>扫码救援</text>
        <br />
        <text class="secondText">扫描桩基二维码，马上排除救援</text>
      </view>
      <view class="inputting">
        <img src="/static/images/8.png" alt />
        <br />
        <text>手动输入</text>
        <br />
        <text class="secondText">相机坏了？手动输入</text>
      </view>
    </view>
    <!-- 救援电话 -->

    <view class="helpPhone">救援电话：2658844</view>
  </view>
</template>

<style lang="scss" scoped>
 .helpcontent {
  display: flex;
  margin: 10rpx 20rpx;
  .scannig,
  .inputting {
    background-color: #626a6d;
    height: 220rpx;
    border: solid 1px;
    border-radius: 10rpx;
    text-align: center;
    color: #fff;
    .secondText {
      font-size: 0.85em;
      width: 100%;
      overflow: hidden;
      text-overflow: ellipsis;
      display: block;
      margin-top:24rpx ;
    }
    img {
      height: 70rpx;
      width: 80rpx;
      margin-top: 14rpx;
    }
  }
  .scannig {
    flex: 1.3;
  }
  .inputting {
    flex: 1;
    margin-left: 18rpx;
  }
}
.helpPhone {
  text-align: center;
  margin: 8rpx 0;
  color: rgb(168, 160, 160);
}
</style>