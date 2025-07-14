

- App Store Connect API
- xcodeMetrics
- xcodeMetrics.ProductData
- xcodeMetrics.ProductData.MetricCategories
-  xcodeMetrics.ProductData.MetricCategories.Metrics 

Object

# xcodeMetrics.ProductData.MetricCategories.Metrics

Data that relates to power and performance measurements for an app, including its datasets, goal keys, metrics identifier, and unit of measurement.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData.MetricCategories.Metrics
```

## Properties

`datasets`

`[`xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets`]`

An array of datasets containing metric values by app version filtered by percentile and device type.

`goalKeys`

`[`xcodeMetrics.ProductData.MetricCategories.Metrics.GoalKeys`]`

An array of terms used to classify a metric value, and the range of values for each classification.

`identifier`

`string`

The identifier of the specific metric within the contained metric category.

`unit`

xcodeMetrics.ProductData.MetricCategories.Metrics.Unit

The metric’s unit of measurement.

## Topics

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets

A set of data containing metric values for each app version, filtered by percentile and device type.

object xcodeMetrics.ProductData.MetricCategories.Metrics.GoalKeys

A classification of a metrics value and the lower- and upper-bound values that qualify a metrics value for the classification.

object xcodeMetrics.ProductData.MetricCategories.Metrics.Unit

A unit of measurement and its display name.

