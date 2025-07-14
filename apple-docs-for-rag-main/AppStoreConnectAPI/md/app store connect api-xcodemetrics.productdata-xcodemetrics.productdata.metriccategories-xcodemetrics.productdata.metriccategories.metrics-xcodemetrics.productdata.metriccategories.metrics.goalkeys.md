

- App Store Connect API
- xcodeMetrics
- 
  - xcodeMetrics
- xcodeMetrics.ProductData
- xcodeMetrics.ProductData.MetricCategories
- xcodeMetrics.ProductData.MetricCategories.Metrics
-  xcodeMetrics.ProductData.MetricCategories.Metrics.GoalKeys 

Object

# xcodeMetrics.ProductData.MetricCategories.Metrics.GoalKeys

A classification of a metrics value and the lower- and upper-bound values that qualify a metrics value for the classification.

App Store Connect API 2.0+

``` source
object xcodeMetrics.ProductData.MetricCategories.Metrics.GoalKeys
```

## Properties

`goalKey`

`string`

The name of the classification, such as `“good”`, `“fair”`, and `“poor”`.

`lowerBound`

`integer`

The lower bound value to qualify for the goal key.

`upperBound`

`integer`

The upper bound value to qualify for the goal key.

## See Also

### Objects

object xcodeMetrics.ProductData.MetricCategories.Metrics.Datasets

A set of data containing metric values for each app version, filtered by percentile and device type.

object xcodeMetrics.ProductData.MetricCategories.Metrics.Unit

A unit of measurement and its display name.

