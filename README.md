# charts-starter-pack

Starter code for a few charting APIs

##Chartkick

Install:

  ```npm install chartkick
  # or
  bower install chartkick```


In HTML head:

```<script src="//www.google.com/jsapi"></script>
<script src="chartkick.js"></script>```

Create a div in HTML:

  ```<div id="chart-1" style="height: 300px;"></div>```

Create the chart in JS:

  ```let chart1 = new Chartkick.PieChart("chart-2", [["Kevin",44],["Strawberry",23],["Rhubard",22],["Apple",21],["Bluberry",13]], {"label":  "Pies"});```

[Chartkick](https://github.com/ankane/chartkick.js)

##Chartist

Install:

  ```bower install chartist --save```


In HTML head:

```<link rel="stylesheet" href="bower_components/chartist/dist/chartist.min.css">```

Create a div in HTML according to Chartist class specifications:

  ```<div id="chartist-bar-chart" class="chart ct-chart well"></div>```

Include Chartist in JS:

  ```let Chartist = require('chartist');```

Create the chart in JS:

  ```let chart2 = new Chartist.Line('#chartist-bar-chart',
  {
    labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri'],
    series: [
      [5, 2, 4, 1, 4.5]
    ],
  }, {
  low: 0,
  showArea: true
});```

[Charist](https://gionkunz.github.io/chartist-js/index.html)

## Highcharts

Install:

  ```npm install highcharts --save```

Create a div in HTML:

  ```<div id="highcharts-chart" class="chart well"></div>```

Include Chartist in JS:

  ```let Highcharts = require('highcharts');```

Create the chart in JS:

  ```let chart1 = new Highcharts.Chart({
  chart: {
      type: 'column',
      renderTo: 'highcharts-chart',
      width: 800
  },
  title: {
      text: 'Ping Pong Wins'
  },
  series: [{
      name: "Wins",
      data: [
          ['A.A.Ron', 8],
          ['Nick', 8],
          ['Kevin', 7],
          ['James', 4],
          ['Jerry', 2]
      ]
  }],
  xAxis: {
      categories: ['A.A.Ron', 'Nick', 'Kevin', 'James', 'Jerry']
  }
});```

[Highcharts](http://www.highcharts.com/)
