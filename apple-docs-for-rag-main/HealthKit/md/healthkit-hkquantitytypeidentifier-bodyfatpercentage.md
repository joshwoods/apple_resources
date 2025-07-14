

- HealthKit
- HKQuantityTypeIdentifier
-  bodyFatPercentage 

Type Property

# bodyFatPercentage

A quantity sample type that measures the user’s body fat percentage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let bodyFatPercentage: HKQuantityTypeIdentifier
```

## Discussion

These samples use percent units (described in HKUnit) and measure discrete values (described in HKQuantityAggregationStyle).

## See Also

### Related Documentation

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKQuantity

An object that stores a value for a given unit.

### Body measurements

static let height: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s height.

static let bodyMass: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s weight.

static let bodyMassIndex: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s body mass index.

static let leanBodyMass: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s lean body mass.

static let waistCircumference: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s waist circumference.

