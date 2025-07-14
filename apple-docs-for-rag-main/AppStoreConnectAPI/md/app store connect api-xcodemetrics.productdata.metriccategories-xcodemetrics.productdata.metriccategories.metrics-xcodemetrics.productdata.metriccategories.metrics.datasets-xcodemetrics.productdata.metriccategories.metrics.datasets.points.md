

- App Store Connect API
- xcodeMetrics
- xcodeMetrics.ProductData
- 
  - xcodeMetrics
  - xcodeMetrics.ProductData
- xcodeMetrics.ProductData.MetricCategories
- xcodeMetrics.ProductData.MetricCategories.Metrics
- xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets
-  xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points 

Object

# xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points

A metric value of a goal for a specific app version, with a breakdown by metric subtypes.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points
```

## Properties

`errorMargin`

`number`

The margin of error estimated based on the sample size and metric type, for metrics with an insufficient data volume. Note: For the system to provide a metric, the number of samples must meet a minimum threshold size. The `errorMargin` is present if a metric meets the minimum, but is inaccurate within a margin. If the metric surpasses a high enough threshold, the `errorMargin` isn’t present.

`goal`

`string`

The metric value’s classification in terms of a goal key, such as `"good",` `"fair"`, or `"poor"`.

`percentageBreakdown`

xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points.PercentageBreakdown

The percentage of the metric value each metric subtype contributes.

`value`

`number`

The metric value. The `unit` field of the xcodeMetrics.ProductData.MetricCategories.Metrics object specifies the units.

`version`

`string`

The app version.

## Topics

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points.PercentageBreakdown

A metric subtype and the percentage of the metric value it contributes.

## See Also

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.FilterCriteria

The device and percentile criteria by which the system filters a metrics dataset.

