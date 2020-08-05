<template>
  <!-- 新闻的容器 -->
  <view class="newsContent">
    <!-- 新闻的每一个item -->
    <view class="newsItem">
      <!-- 弹性设置 -->
      <view class="newsInWrap">
        <view class="newsWorld">
            2人身亡！泸高速惨烈车祸，2车事故为何变成5车猛烈追尾？
        </view>
        <view class="newsImg">
            <img src="/static/images/9.png" alt="">
        </view>
      </view>
      <!-- Item的脚注 -->
      <view class="newsFooter">
        <text>5000评论</text>
        <text class="secondWorld">昨天13.42</text>
      </view>
    </view>
  </view>
</template>

<style lang="scss" scoped>
.newsContent{
    margin-top: 30rpx;
}
.newsItem {
    height: 220rpx;
    border: solid 1rpx rgb(163, 156, 156);
    position: relative;
    padding: 20rpx;
   .newsInWrap {
    display: flex;
    justify-content: space-around;
    .newsWorld {
      flex: 7;
    }
    .newsImg {
      flex: 4;
      img{ 
          width: 100%;
          height: 200rpx;
        }
    }
  }
  .newsFooter{
      position: absolute;
      bottom: 20rpx;
      font-size: 0.6em;
      color: rgb(179, 168, 168);
      .secondWorld{
          padding-left:30rpx ;
      }
     
  }
}
</style>