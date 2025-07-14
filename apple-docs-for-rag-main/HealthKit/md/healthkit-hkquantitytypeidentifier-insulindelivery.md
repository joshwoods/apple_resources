

- HealthKit
- HKQuantityTypeIdentifier
-  insulinDelivery 

Type Property

# insulinDelivery

A quantity sample that measures the amount of insulin delivered.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
static let insulinDelivery: HKQuantityTypeIdentifier
```

## Discussion

These samples use international units (IU) (described in HKUnit) and measure cumulative values (described in HKQuantityAggregationStyle).

## Topics

### Metadata Keys

let HKMetadataKeyInsulinDeliveryReason: String

The medical reason for administering insulin.

## See Also

### Related Documentation

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKQuantity

An object that stores a value for a given unit.

### Lab and test results

static let bloodAlcoholContent: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s blood alcohol content.

static let bloodGlucose: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s blood glucose level.

static let electrodermalActivity: HKQuantityTypeIdentifier

A quantity sample type that measures electrodermal activity.

static let forcedExpiratoryVolume1: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of air that can be forcibly exhaled from the lungs during the first second of a forced exhalation.

static let forcedVitalCapacity: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of air that can be forcibly exhaled from the lungs after taking the deepest breath possible.

static let inhalerUsage: HKQuantityTypeIdentifier

A quantity sample type that measures the number of puffs the user takes from their inhaler.

static let numberOfTimesFallen: HKQuantityTypeIdentifier

A quantity sample type that measures the number of times the user fell.

static let peakExpiratoryFlowRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s maximum flow rate generated during a forceful exhalation.

static let peripheralPerfusionIndex: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s peripheral perfusion index.

