

- HealthKit
- HKQuantityType
-  is(compatibleWith:) 

Instance Method

# is(compatibleWith:)

Returns a Boolean value that indicates whether the quantity type is compatible with the given unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func `is`(compatibleWith unit: HKUnit) -> Bool
```

## Parameters 

`unit`  

The HealthKit unit to be checked.

## Return Value

YES if the quantity type is compatible with the given unit; otherwise, NO.

## Discussion

When creating a HealthKit quantity sample, the sample’s type and quantity object must use compatible units. For more information, see HKQuantity.

## See Also

### Accessing Quantity Type Data

var aggregationStyle: HKQuantityAggregationStyle

The aggregation style for the given quantity type.

enum HKQuantityAggregationStyle

Constant values that describe how quantities can be aggregated over time.

