

- App Store Connect API
- xcodeMetrics
- xcodeMetrics.ProductData
-  xcodeMetrics.ProductData.MetricCategories 

Object

# xcodeMetrics.ProductData.MetricCategories

A metric category and its associated array of data and measurements.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData.MetricCategories
```

## Properties

`identifier`

MetricCategory

The category of the metric that this product data is about.

`metrics`

`[`xcodeMetrics.ProductData.MetricCategories.Metrics`]`

An array of data and measurements for the metric category specified by the `identifier`.

## Topics

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics

Data that relates to power and performance measurements for an app, including its datasets, goal keys, metrics identifier, and unit of measurement.

