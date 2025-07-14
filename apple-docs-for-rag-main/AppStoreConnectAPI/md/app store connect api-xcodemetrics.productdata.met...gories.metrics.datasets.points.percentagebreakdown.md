

- App Store Connect API
- xcodeMetrics
- xcodeMetrics.ProductData
- xcodeMetrics.ProductData.MetricCategories
- 
  - xcodeMetrics
  - xcodeMetrics.ProductData
  - xcodeMetrics.ProductData.MetricCategories
- xcodeMetrics.ProductData.MetricCategories.Metrics
- xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets
- xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points
-  xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points.PercentageBreakdown 

Object

# xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points.PercentageBreakdown

A metric subtype and the percentage of the metric value it contributes.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points.PercentageBreakdown
```

## Properties

`subSystemLabel`

`string`

A string that describes the metric subtype, which provides more information about the measurement.

`value`

`number`

The percentage of the metric value the metric subtype contributes. Values are between `0` and `100`.

