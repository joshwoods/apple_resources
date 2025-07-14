

- HealthKit
- HKQuantityTypeIdentifier
-  dietaryFatTotal 

Type Property

# dietaryFatTotal

A quantity sample type that measures the total amount of fat consumed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let dietaryFatTotal: HKQuantityTypeIdentifier
```

## Discussion

These samples include polyunsaturated, monounsaturated, and saturated fats. These samples use mass units (described in HKUnit) and measure cumulative values (described in HKQuantityAggregationStyle).

## See Also

### Related Documentation

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKQuantity

An object that stores a value for a given unit.

### Macronutrients

static let dietaryEnergyConsumed: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of energy consumed.

static let dietaryCarbohydrates: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of carbohydrates consumed.

static let dietaryFiber: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of fiber consumed.

static let dietarySugar: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of sugar consumed.

static let dietaryFatMonounsaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of monounsaturated fat consumed.

static let dietaryFatPolyunsaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of polyunsaturated fat consumed.

static let dietaryFatSaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of saturated fat consumed.

static let dietaryCholesterol: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of cholesterol consumed.

static let dietaryProtein: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of protein consumed.

