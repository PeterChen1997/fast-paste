<template>
  <view class="container">

    <view class="title">
      <text>快速粘贴板</text>
      <text>Fast Paste</text>
    </view>

    <view class="options">
      <text @tap="jumpAdd">新建记录</text>
      <text @tap="jumpHistory">历史记录</text>
      <text @tap="jumpCollect">收藏夹</text>
    </view>

    <view class="statement">
      <text>Fast Paste</text>
      <text>develop by Peter Chen</text>
    </view>
  </view>
</template>

<script>
import Taro from '@tarojs/taro'

export default {
  name: 'Index',
  components: {
  },
  methods: {
    jumpAdd() {
      console.log('jumpadd')
      Taro.navigateTo({
        url: '/pages/add/index'
      })
    },
    jumpHistory() {
      Taro.navigateTo({
        url: '/pages/history/index'
      })
    },
    jumpCollect() {
      Taro.navigateTo({
        url: '/pages/collect/index'
      })
    },
  }
}
</script>

<style>
.container {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.title {
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
  
  height: 30vh;
  font-size: 70px;
}

.options {
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: space-around;

  height: 50vh;
  font-size: 50px;
}

.statement {
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;

  height: 20vh;
  font-size: 30px;
}
</style>
