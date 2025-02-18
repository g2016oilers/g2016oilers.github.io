---
title: Home
layout: home
title: Tournaments
layout: home
title: Statistics
layout: home
---
Welcome to the home of the Stavanger Oilers boys 2016 hockey team

----
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Visualization</title>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
</head>
<body>
    <canvas id="myChart" width="400" height="200"></canvas>
    <script>
        const ctx = document.getElementById('myChart').getContext('2d');
        var mixedChart = new Chart(ctx, {
            type: 'bar',
            data: {
                datasets: [{
                    label: 'Team Goals',
                    data: [4, 4, 2, 2, 7, 11, 7, 3, 9, 8, 3],
                    order: 1
            }, {
                label: 'Team Passes',
                data: [10, 28, 18, 24, 32, 29, 18, 21, 16, 17, 12],
                type: 'line',
                order: 2
        }],
        labels: ['G1: Skedsmo', 'G2: Lørenskog', 'G3: Lørenskog', 'G4: Comet', 'G5: Skedsmo', 'G6: Astor', 'G7: Rosenborg', 'G8: Rosenborg', 'G9: Astor', 'G10: Comet', 'G11: Lærenskog']
    },
       options: {
                scales: {
                    y: {
                        beginAtZero: true
                    }
                }
            }
        });
    </script>
<div id="myDiv" style="width: 100%; height: 100%;"></div>
<script>
  var data = [{
    x: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
    y: [4, 4, 3, 6, 7, 10, 12, 9, 10, 4, 3],
    mode: 'markers',
    type: 'scatter'
  }];

  Plotly.newPlot('myDiv', data);
</script>
</body>
</html>
----

[^1]: [It can take up to 10 minutes for changes to your site to publish after you push the changes to GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site).

[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[README]: https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md
[Jekyll]: https://jekyllrb.com
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[use this template]: https://github.com/just-the-docs/just-the-docs-template/generate
