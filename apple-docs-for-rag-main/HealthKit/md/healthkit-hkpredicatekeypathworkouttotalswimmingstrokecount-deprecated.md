

- HealthKit
-  HKPredicateKeyPathWorkoutTotalSwimmingStrokeCount Deprecated

Global Variable

# HKPredicateKeyPathWorkoutTotalSwimmingStrokeCount

The key path for accessing the number of strokes during a swimming workout.

iOS 10.0–18.0DeprecatediPadOS 10.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 3.0–11.0Deprecated

``` source
let HKPredicateKeyPathWorkoutTotalSwimmingStrokeCount: String
```

Deprecated

Use predicateForWorkoutActivitiesWithOperatorType:quantityType:sumQuantity: passing the HKQuantityType for HKQuantityTypeIdentifierSwimmingStrokeCount

## See Also

### Workout keys

let HKPredicateKeyPathWorkout: String

The key path for accessing the object’s workout inside a predicate format string.

let HKPredicateKeyPathWorkoutType: String

The key path for accessing the workout’s type.

let HKPredicateKeyPathWorkoutDuration: String

The key path for accessing the workout’s duration.

let HKPredicateKeyPathWorkoutAverageQuantity: String

The key path for accessing workouts with a matching average quantity.

let HKPredicateKeyPathWorkoutMaximumQuantity: String

The key path for accessing workouts with a matching maximum quantity.

let HKPredicateKeyPathWorkoutMinimumQuantity: String

The key path for accessing workouts with a matching minimum quantity.

let HKPredicateKeyPathWorkoutSumQuantity: String

The key path for accessing workouts with a matching sum.

let HKPredicateKeyPathWorkoutTotalDistance: String

The key path for accessing the workout’s total distance.

Deprecated

let HKPredicateKeyPathWorkoutTotalEnergyBurned: String

The key path for accessing the workout’s total energy burned.

Deprecated

let HKPredicateKeyPathWorkoutTotalFlightsClimbed: String

The key path for accessing the total number of flights of stairs climbed during the workout.

Deprecated

