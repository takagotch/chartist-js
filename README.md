### chartist-js
---
https://github.com/gionkunz/chartist-js

https://gionkunz.github.io/chartist-js/
```js
var data = {
  labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri'],
  series: [
    [5, 2, 4, 2, 0]
  ]
};
new Chartist.Line('.ct-chart', data);

var data = {  labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri'],
              series: [
                [5, 2, 4, 2, 0]
              ]
};
var options = {
  width: 300,
  height: 200
};

new Chartist.Line('.ct-chart', data, options);

var data = {
  labels: ['A', 'B', 'C'],
  series: [[10, 8, 14]]
};

var data = {
  labels: ['A', 'B', 'C'],
  series: [[
    {x: undefined, y: 10},
    {x: undefined, y: 8},
    {x: undefined, y: 14}
  ]]
};
```

```
bower install chartist --save
cp bower_components/chartist/dist/scss/settings/_chartist-settings.scss styles
```

```
<html>
  <head>
    <title></title>
    <link rel="stylesheet" href="bower_components/chartist/dist/chartist.min.css">
  </head>
  <body>
    <script src="bower_components/chartist/dist/chartist.min.js"></script>
  </body>
</html>

<div class="ct-chart ct-persect-fourth">
</div>

<div class="ct-chart ct-golden-section" id="chart1"></div>
<div class="ct-chart ct-golden-section" id="chart2"></div>
<script>
  new Chartist.Line('#chart1', {
    labels: [1, 2, 3, 4], 
    series: [[100, 120, 180, 200]]
  });
  new Chartist.Bar('#chart2', {
    labels: [1, 2, 3, 4],
    series: [[5, 2, 8, 3]]
  });
</script>

```

```css
@import "_my-chartist-settings.scss";
@import "chartist/dist/scss/chartist.scss";

.ct-series-a .ct-line {
  stroke: red;
  stroke-width: 5px;
  stroke-dasharray: 10px 20px;
}
.ct-series-a .ct-point {
  stroke: red;
  stroke-width: 20px;
  stroke-linecap: square;
}

.ct-series-a .ct-bar {
  stroke: red;
  stroke-width: 20px;
  stroke-dahsarray: 20px;
  stroke-linecap: round;
}

.ct-series-a .ct-slice-pie {
  fill: hsl(120, 40%, 60%);
  stroke: white;
  stroke-width: 4px;
}

.ct-series-a .ct-slice-donut {
  stroke: blue;
  stroke-width: 5px !important;
  stroke-linecap: round;
}

.ct-series-a .ct-line,
.ct-series-a .ct-point {
  stroke: blue;
}
.ct-series-b .ct-line,
.ct-series-b .ct-point {
  stroke: green;
}
```



