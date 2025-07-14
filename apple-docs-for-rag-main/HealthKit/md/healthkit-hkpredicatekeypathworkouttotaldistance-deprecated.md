

- HealthKit
-  HKPredicateKeyPathWorkoutTotalDistance Deprecated

Global Variable

# HKPredicateKeyPathWorkoutTotalDistance

The key path for accessing the workout’s total distance.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.0+macOS 13.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
let HKPredicateKeyPathWorkoutTotalDistance: String
```

Deprecated

Use predicateForWorkoutActivitiesWithOperatorType:quantityType:sumQuantity: passing the HKQuantityType for the desired distance type

## See Also

### Specifying predicate key paths

let HKPredicateKeyPathWorkoutType: String

The key path for accessing the workout’s type.

let HKPredicateKeyPathWorkoutDuration: String

The key path for accessing the workout’s duration.

let HKPredicateKeyPathWorkoutTotalEnergyBurned: String

The key path for accessing the workout’s total energy burned.

Deprecated

let HKPredicateKeyPathWorkoutAverageQuantity: String

The key path for accessing workouts with a matching average quantity.

let HKPredicateKeyPathWorkoutMaximumQuantity: String

The key path for accessing workouts with a matching maximum quantity.

let HKPredicateKeyPathWorkoutMinimumQuantity: String

The key path for accessing workouts with a matching minimum quantity.

let HKPredicateKeyPathWorkoutSumQuantity: String

The key path for accessing workouts with a matching sum.

