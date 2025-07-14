

- HealthKit
- HKWorkout
-  totalEnergyBurned Deprecated

Instance Property

# totalEnergyBurned

The total active energy burned during the workout.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 2.0–11.0Deprecated

``` source
var totalEnergyBurned: HKQuantity? { get }
```

Deprecated

Use allStatistics or statistics(for:) instead.

## Mentioned in 

Adding samples to a workout

## Discussion

This property contains a quantity using energy units, or `nil`.

Note

Provide a total energy burned value whenever the active calories burned is relevant to the workout type. In addition, add active energy burned samples to a workout using the add(_:to:completion:) method. These samples should sum up to the total energy, while providing detailed information about how the intensity changes over the duration of the workout.

## See Also

### Related Documentation

func splitTotalEnergy(HKQuantity, start: Date, end: Date, resultsHandler: (HKQuantity?, HKQuantity?, (any Error)?) -> Void)

Calculates the active and resting energy burned based on the total energy burned over the given duration.

Deprecated

### Accessing workout data

var duration: TimeInterval

The workout’s duration.

var workoutActivityType: HKWorkoutActivityType

The type of activity performed during the workout.

var workoutActivities: [HKWorkoutActivity]

var workoutEvents: [HKWorkoutEvent]?

An array of workout event objects.

func statistics(for: HKQuantityType) -> HKStatistics?

Returns the workout’s statistics for the provided quantity type.

var allStatistics: [HKQuantityType : HKStatistics]

A dictionary that contains all the statistics for the workout.

var totalDistance: HKQuantity?

The total distance traveled during the workout.

Deprecated

var totalFlightsClimbed: HKQuantity?

The total number of flights of stairs climbed during the workout.

Deprecated

var totalSwimmingStrokeCount: HKQuantity?

The total stroke count for the workout.

Deprecated

