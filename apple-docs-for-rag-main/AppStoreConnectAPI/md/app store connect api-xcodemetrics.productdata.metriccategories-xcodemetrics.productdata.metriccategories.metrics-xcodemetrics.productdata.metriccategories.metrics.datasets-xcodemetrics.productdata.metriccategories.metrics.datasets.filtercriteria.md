

- App Store Connect API
- xcodeMetrics
- xcodeMetrics.ProductData
- 
  - xcodeMetrics
  - xcodeMetrics.ProductData
- xcodeMetrics.ProductData.MetricCategories
- xcodeMetrics.ProductData.MetricCategories.Metrics
- xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets
-  xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.FilterCriteria 

Object

# xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.FilterCriteria

The device and percentile criteria by which the system filters a metrics dataset.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.FilterCriteria
```

## Properties

`device`

`string`

The device type that the measurement is collected on.

`deviceMarketingName`

`string`

The human-readable string containing the device name.

`percentile`

`string`

A percentile of users affected by the metric value. The 50th percentile represents a typical user experience. The 90th percentile represents the user experience when the metric value is the highest or lowest, depending on the metric.

## See Also

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points

A metric value of a goal for a specific app version, with a breakdown by metric subtypes.

