# Radar chart
This radar chart allows you to add sections as you wish, and change their values. The labels of every section can also be changed.

## A simple guide
Here's a simple tutorial on how to use it.

```js
const data = {
  labels: ['Section 1', 'Section 2', 'Section 3', 'Section 4', 'Section 5', 'Section 6'],
  datasets: [{
    label: 'Radar Chart',
    data: [3, 1, 2, 3, 1, 3],
    backgroundColor: 'rgba(75, 192, 192, 0.2)',
    borderColor: 'rgba(75, 192, 192, 1)',
    borderWidth: 1
  }]
};
```

#### Adding sections
To add a section, you can just add another label to the `labels` dataset and another value to the `data` dataset.

#### Changing the color
To change the color, you can just edit the `backgroundColor` and `borderColor` properties.

#### Adding another chart
```js
const ctx2 = document.getElementById('snowflakeChart2').getContext('2d');
const data2 = {
  labels: ['Category 1', 'Category 2', 'Category 3', 'Category 4', 'Category 5', 'Category 6', 'Category 7', 'Category 8', 'Category 9', 'Category 10'],
  datasets: [{
    label: 'Snowflake Analysis 2',
    data: [2.2, 3.6, 4.3, 1.8, 3.0, 2.7, 4.5, 1.5, 3.2, 2.9],
    backgroundColor: 'rgba(192, 75, 75, 0.2)',
    borderColor: 'rgba(192, 75, 75, 1)',
    borderWidth: 1
    }]
};

const options2 = {
  scales: {
    r: {
      angleLines: {
        display: false
      },
      suggestedMin: 0,
      suggestedMax: 5,
      ticks: {
        display: false
      },
      pointLabels: {
        color: '#fff',
        font: {
          family: 'Plus Jakarta Sans',
          size: 14
        }
      }
    }
  },
  plugins: {
    legend: {
      display: false
    }
  }
};

const snowflakeChart2 = new Chart(ctx2, {
  type: 'radar',
  data: data2,
  options: options2
});
```
To add another chart, you can simply copy the code above, and adding it inside the `script` tag ,editing the number, for ex. adding a third chart would mean you use `ctx3` instead of just `ctx`.

## Website
You can access it [here.](https://duckingtonthe3rd.github.io/Radar-chart/)
