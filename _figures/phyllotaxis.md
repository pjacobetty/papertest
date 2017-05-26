---
layout: figure
order: 2
label: Figure 2
title: "A visualisation"
description: "A visualisation of the data"
image: "data/phyllotaxis/figure.png"
---

<script src="http://www.chartjs.org/dist/2.6.0/Chart.bundle.js"></script>    <style>    canvas {        -moz-user-select: none;        -webkit-user-select: none;        -ms-user-select: none;    }    </style><canvas id="myChart" width="15" height="15"></canvas><script>var ctx = document.getElementById("myChart").getContext('2d');var myChart = new Chart(ctx, {    type: 'bar',    data: {        labels: ["Red", "Blue", "Yellow", "Green", "Purple", "Orange"],        datasets: [{            label: '# of Votes',            data: [12, 19, 3, 5, 2, 3],            backgroundColor: [                'rgba(255, 99, 132, 0.2)',                'rgba(54, 162, 235, 0.2)',                'rgba(255, 206, 86, 0.2)',                'rgba(75, 192, 192, 0.2)',                'rgba(153, 102, 255, 0.2)',                'rgba(255, 159, 64, 0.2)'            ],            borderColor: [                'rgba(255,99,132,1)',                'rgba(54, 162, 235, 1)',                'rgba(255, 206, 86, 1)',                'rgba(75, 192, 192, 1)',                'rgba(153, 102, 255, 1)',                'rgba(255, 159, 64, 1)'            ],            borderWidth: 1        }]    },    options: {        scales: {            yAxes: [{                ticks: {                    beginAtZero:true                }            }]        }    }});</script>
