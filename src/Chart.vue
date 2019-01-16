<template>
  <div id="container" style="width:100%; height:400%"></div>
</template>
<script>
export default {
  mounted() {
    Highcharts.chart('container', {
      chart: {
        type: 'bar'
      },
      title: {
        text: 'Fruite Consumption'
      },
      xAxis: {
        categories: ['Apples', 'Bananas', 'Orange']
      },
      yAxis: {
        title: {
          text: 'Fruit eaten'
        }
      },
      series: [{
        name: 'Jane',
        data: [1, 0, 4]
      }, {
        name: 'Jieun',
        data: [5, 7, 3]
      }]
    })
  }
}
</script>
