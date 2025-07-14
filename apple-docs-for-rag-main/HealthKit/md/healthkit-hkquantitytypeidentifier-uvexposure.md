

- HealthKit
- HKQuantityTypeIdentifier
-  uvExposure 

Type Property

# uvExposure

A quantity sample type that measures the user’s exposure to UV radiation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let uvExposure: HKQuantityTypeIdentifier
```

## Discussion

These samples use count units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle). The sample’s value represents the UV index that the user was exposed to during the sample’s duration.

## See Also

### Related Documentation

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKQuantity

An object that stores a value for a given unit.

