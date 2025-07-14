

- App Store Connect API
- xcodeMetrics
- 
  - xcodeMetrics
- xcodeMetrics.ProductData
- xcodeMetrics.ProductData.MetricCategories
- xcodeMetrics.ProductData.MetricCategories.Metrics
-  xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets 

Object

# xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets

A set of data containing metric values for each app version, filtered by percentile and device type.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets
```

## Properties

`filterCriteria`

xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.FilterCriteria

The device and percentile criteria by which the dataset is filtered.

`points`

`[`xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points`]`

An array containing metric values for each app version.

## Topics

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.FilterCriteria

The device and percentile criteria by which the system filters a metrics dataset.

object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets.Points

A metric value of a goal for a specific app version, with a breakdown by metric subtypes.

## See Also

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics.GoalKeys

A classification of a metrics value and the lower- and upper-bound values that qualify a metrics value for the classification.

object xcodeMetrics.ProductData.MetricCategories.Metrics.Unit

A unit of measurement and its display name.

