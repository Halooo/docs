Chart.js vs Echarts3

## Similarities

- both using canvas
- enough types of charts to fulfill feature requirements
- both not encapsulated as React component
- Not much room for customization
- Active community and people are still contributing

## Repository Comparison

![repo](./repo.png)

## Demos and API Documentation

[Echarts Demo](https://ecomfe.github.io/echarts-examples/public/index.html)

![echarts demo](./echart_demo.png)

[Echarts Documentation](https://ecomfe.github.io/echarts-doc/public/en/api.html#echarts)

![echarts api](./echarts_api.png)

[Chart.js Demo](http://www.chartjs.org/samples/latest/)

![chartjs demo](./chartjs_demo1.png)





![chartjs demo](./chartjs_demo2.png)





![chartjs demo](./chartjs_demo3.png)



![chartjs demo](./chartjs_api.png)





| Echarts                                  | Chartjs                                  |
| ---------------------------------------- | ---------------------------------------- |
| Clear API and Options documentation      | Less clear documentation                 |
| Clear and detailed demo, but less resource on Google | Simple demo, but lots of solutions can be Googled |
| Able to handle big data                  | Able to handle big data                  |
| BSD 3-Clause License                     | MIT License                              |
| 70% of issues on Github are in Chinese (with minimum English Translation) | Active English community                 |



## Package Size

| Echarts | Supports including charts and components on demand | minified |
| ------- | ---------------------------------------- | -------- |
| Common  | line bar pie scatter legend tooltip toolbox markLine markPoint markArea dataZoom | 400k     |
| Simple  | line bar pie                             | 263k     |
| Full    | Includes all charts and components       | 651k     |

```javascript
// include ECharts main module
const echarts = require('echarts/lib/echarts');
// include bar chart tooltip and title component
require('echarts/lib/chart/bar');
require('echarts/lib/component/tooltip');
require('echarts/lib/component/title');
// ~170KB
```

[Available Echarts modules](https://github.com/ecomfe/echarts/blob/master/index.js)


| Chart.js | minified | gzipped |
| -------- | -------- | ------- |
|          | 363k     | 105k    |

```javascript
const Chart = require('chart.js');
let myChart = new Chart(ctx, {...});
```

[Chart.js Releases](https://github.com/chartjs/Chart.js/releases)



Suggestion:

We can combine the use of D3.js with the canvas solution because SVGs from D3.js are good for heavy user interaction components. 

Also Check out [VICTORY](https://formidable.com/open-source/victory/gallery) by formidable (MIT), it is a chart library designed for React. 