<template>
  <div class="left-chart-2">
    <div class="lc2-header">公司项目动态</div>
      <div class="text_hrel">
    <div @click="goPage1('http://datav.jiaminghi.com/')">对手动态1</div>
    <div @click="goPage2('https://github.com/')">对手动态2</div>
    <div @click="goPage3('http:///www.baidu.com')">对手动态3</div>
    <div @click="goPage4('http://www.xinhuanet.com/')">对手动态4</div>
    <dv-decoration-2 style="height:10px;" />
    </div>
    <!-- <div class="lc2-details">设备运行总数<span>245</span></div>
    <dv-charts class="lc2-chart" :option="option" /> -->
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
.left-chart-2 {
  width: 100%;
  height: 30%;
  display: flex;
  flex-direction: column;

  .lc2-header {
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

  // .lc2-details {
  //   height: 40px;
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

  // .lc2-chart {
  //   height: calc(~"100% - 80px");
  // }
}
</style>
