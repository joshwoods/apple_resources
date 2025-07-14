

- HealthKit
- HKQuantityAggregationStyle
-  discrete Deprecated

Type Property

# discrete

Discrete samples may be averaged over time.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
static var discrete: HKQuantityAggregationStyle { get }
```

Deprecated

Use HKQuantityAggregationStyle.discreteArithmetic instead.

## Discussion

You typically use discrete types to monitor the change in the value over time. For example, body mass, heart rate, temperature, and respiratory rate are all discrete quantity types. You can also query for the minimum or maximum value in a given time period.

