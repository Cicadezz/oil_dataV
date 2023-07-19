<template>

  <div class="bottom-charts">
    <div class="bc-header">
      <div>最新新闻咨询</div>
      <div @click="goPage1('http://datav.jiaminghi.com/')">点击此处跳转至新闻页面1</div>
      <div @click="goPage2('https://github.com/')">点击此处跳转至新闻页面2</div>
      <div @click="goPage3('http:///www.baidu.com')">点击此处跳转至新闻页面3</div>
      <div @click="goPage4('http://www.xinhuanet.com/')">点击此处跳转至新闻页面4</div>
    </div>

  </div>
</template>

<script>
export default {
  methods: {
    goPage1 (url) {
      window.open(url, '_blank')
    },
    goPage2 (url) {
      window.open(url, '_blank')
    },
    goPage3 (url) {
      window.open(url, '_blank')
    },
    goPage4 (url) {
      window.open(url, '_blank')
    }
  }
}
</script>

<style lang="less">
.bottom-charts {
  width: 100%;
  height: 100%;
  display: flex;
  position: relative;

  .bc-header{
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    font-size:20px;
    text-align: center;
  }
}
</style>
