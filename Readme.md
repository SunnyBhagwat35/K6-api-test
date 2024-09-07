## Basic Run Command
``k6 run filename.js``

## Get results and output into different file
[click here to see the document](https://grafana.com/docs/k6/latest/results-output/real-time/)
 
K6 allows you to export the test results in various formats, such as JSON, CSV, and others. Lets output it into json.

``k6 run --out json=results.json filename.js``

Can also export the results to InfluxDB and visualize them using Grafana. This setup allows for real-time monitoring and in-depth analysis. Here's a basic example:

``k6 run --out influxdb=http://localhost:8086/k6db postReq.js
``




