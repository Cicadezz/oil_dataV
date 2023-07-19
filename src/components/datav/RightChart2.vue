<template>
  <div class="right-chart-2">
    <div class="rc1-header">各中心招投标数量</div>

    <div class="rc1-chart-container">
      <!-- <div class="left">
        <div class="number">415</div>
        <div>招投标总数</div>
      </div> -->
      <dv-scroll-ranking-board class="right" :config="config"/>
      <!-- <dv-capsule-chart class="right" :config="config" /> -->
    </div>
  </div>
</template>

<script>

export default {
  name: 'RightChart1',
  data () {
    return {
      config: {
        data: [
          {
            name: '中心1',
            value: 55
          },
          {
            name: '中心2',
            value: 120
          },
          {
            name: '中心3',
            value: 78
          },
          {
            name: '中心4',
            value: 66
          },
          {
            name: '中心5',
            value: 80
          },
          {
            name: '中心6',
            value: 45
          },
          {
            name: '中心7',
            value: 29
          }
        ]
      }
    }
  }
}
</script>

<style lang="less">
.right-chart-2 {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;

  .rc1-header {
    text-align: center;
    font-size: 24px;
    font-weight: bold;
    height: 30px;
    line-height: 30px;
  }

  .rc1-chart-container {
    flex: 1;
    display: flex;
  }

  // .left {
  //   width: 30%;
  //   font-size: 16px;
  //   display: flex;
  //   flex-direction: column;
  //   justify-content: center;
  //   align-items: center;

  //   .number {
  //     font-size: 34px;
  //     color: #096dd9;
  //     font-weight: bold;
  //     margin-bottom: 30px;
  //   }
  // }

  .right {
    flex: 1;
    padding-bottom: 20px;
    padding-right: 10px;
    padding-left: 10px;
    box-sizing: border-box;
    font-weight: bolder;
  }
}
</style>

<!-- // export default {
//   name: 'RightChart2',
//   data () {
//     return {
//       option: {
//         series: [
//           {
//             type: 'pie',
//             data: [
//               { name: '中心1', value: 93 },
//               { name: '中心2', value: 66 },
//               { name: '中心3', value: 52 },
//               { name: '中心4', value: 34 },
//               { name: '中心5', value: 22 }
//             ],
//             radius: ['45%', '65%'],
//             insideLabel: {
//               show: false
//             },
//             outsideLabel: {
//               labelLineEndLength: 10,
//               formatter: '{percent}%\n{name}',
//               style: {
//                 fontSize: 14,
//                 fill: '#fff'
//               }
//             }
//           }
//         ],
//         color: ['#00baff', '#3de7c9', '#fff', '#ffc530', '#469f4b']
//       }
//     }
//   }
// }
//

// <style lang="less">
// .right-chart-2 {
//   width: 100%;
//   height: 100%;
//   display: flex;
//   flex-direction: column;

//   .rc1-header {
//     font-size: 24px;
//     font-weight: bold;
//     height: 30px;
//     line-height: 30px;
//   }

//   .rc1-chart-container {
//     flex: 1;
//     display: flex;
//   }

//   .left {
//     width: 30%;
//     font-size: 16px;
//     display: flex;
//     flex-direction: column;
//     justify-content: center;
//     align-items: center;

//     .number {
//       font-size: 34px;
//       color: #096dd9;
//       font-weight: bold;
//       margin-bottom: 30px;
//     }
//   }

//   .right {
//     flex: 1;
//     padding-bottom: 20px;
//     padding-right: 20px;
//     box-sizing: border-box;
//   }
// }
// </style> -->
