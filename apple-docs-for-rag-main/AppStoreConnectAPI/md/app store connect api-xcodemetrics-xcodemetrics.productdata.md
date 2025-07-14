

- App Store Connect API
- xcodeMetrics
-  xcodeMetrics.ProductData 

Object

# xcodeMetrics.ProductData

The metrics information of an app on a specific platform.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData
```

## Properties

`metricCategories`

`[`xcodeMetrics.ProductData.MetricCategories`]`

An array of metrics by category.

`platform`

`string`

The Apple platform on which the system gathered the metrics about your app.

## Topics

### Objects

object xcodeMetrics.ProductData.MetricCategories

A metric category and its associated array of data and measurements.

## See Also

### Objects

object xcodeMetrics.Insights

Analysis of power and performance data collected for your app that includes regressions and trends.

