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

## Website
You can access it [here.](https://duckingtonthe3rd.github.io/Radar-chart/)
