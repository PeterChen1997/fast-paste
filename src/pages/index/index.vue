<template>
  <view class="container">

    <view class="title">
      <text>快速粘贴板</text>
      <text>Fast Paste</text>
    </view>

    <view class="options">
      <text>新建记录</text>
      <text>历史记录</text>
      <text>收藏夹</text>
    </view>

    <view class="statement">
      <text>Fast Paste</text>
      <text>develop by Peter Chen</text>
    </view>
  </view>
</template>

<script>

export default {
  name: 'Index',
  components: {

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
  height: 300px;
}

.options {
  display: flex;
  flex-direction: column;

  height: 550px;
}

.statement {
  height: 300px;
}
</style>
