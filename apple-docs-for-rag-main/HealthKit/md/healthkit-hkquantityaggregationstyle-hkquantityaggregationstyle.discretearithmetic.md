

- HealthKit
- HKQuantityAggregationStyle
-  HKQuantityAggregationStyle.discreteArithmetic 

Case

# HKQuantityAggregationStyle.discreteArithmetic

Discrete samples that can be averaged over time using an arithmetic mean.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case discreteArithmetic
```

## Discussion

Use discrete types to monitor changes in a value over time. Body mass, heart rate, temperature, and respiratory rate are all discrete quantity types. You can also query for the minimum or maximum value in a given time period.

## See Also

### Aggregation Styles

case cumulative

Cumulative samples that can be summed over time.

case discreteTemporallyWeighted

Discrete samples that can be averaged over a time interval using a temporally weighted integration function.

case discreteEquivalentContinuousLevel

Discrete samples that can be combined over a time interval by computing the equivalent continuous sound level.

