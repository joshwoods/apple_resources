

- HealthKit
- HKQuantityType
-  aggregationStyle 

Instance Property

# aggregationStyle

The aggregation style for the given quantity type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var aggregationStyle: HKQuantityAggregationStyle { get }
```

## Discussion

For more information on aggregation styles, see HKQuantityAggregationStyle.

## See Also

### Accessing Quantity Type Data

enum HKQuantityAggregationStyle

Constant values that describe how quantities can be aggregated over time.

func `is`(compatibleWith: HKUnit) -> Bool

Returns a Boolean value that indicates whether the quantity type is compatible with the given unit.

