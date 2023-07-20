<template>
  <div class="left-chart-1">
    <div class="lc1-header">竞争对手动态</div>
      <div class="text_hrel">
    <div @click="goPage1('http://datav.jiaminghi.com/')">对手动态1</div>
    <div @click="goPage2('https://github.com/')">对手动态2</div>
    <div @click="goPage3('http:///www.baidu.com')">对手动态3</div>
    <div @click="goPage4('http://www.xinhuanet.com/')">对手动态4</div>
    <dv-decoration-8 style="width:100%;height:50px;" />
  </div>
    <!-- <div class="lc1-details">本月事件总数<span>220</span></div> -->
    <!-- <dv-capsule-chart class="lc1-chart" :config="config" />-->

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
.left-chart-1 {
  width: 100%;
  height: 37%;
  display: flex;
  flex-grow: 0;
  flex-direction: column;

  .lc1-header {
    text-align: center;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 30px;
    margin-bottom: 20px;
  }
    .text_hrel{
    text-align: center;
    height: 40px;
    display: block ;
    justify-content: center;
    align-items: center;
    font-size: 30px;
    }

  // .lc1-details {
  //   height: 50px;
  //   font-size: 16px;
  //   display: flex;
  //   align-items: center;
  //   text-indent: 20px;

  //   span {
  //     color: #096dd9;
  //     font-weight: bold;
  //     font-size: 35px;
  //     margin-left: 20px;
  //   }
  // }

  // .lc1-chart {
  //   flex: 1;
  // }
}
</style>
