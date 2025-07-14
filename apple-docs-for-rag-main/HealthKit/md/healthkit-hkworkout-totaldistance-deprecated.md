

- HealthKit
- HKWorkout
-  totalDistance Deprecated

Instance Property

# totalDistance

The total distance traveled during the workout.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.0+macOS 13.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
var totalDistance: HKQuantity? { get }
```

Deprecated

Use allStatistics or statistics(for:) instead.

## Mentioned in 

Adding samples to a workout

## Discussion

This property contains a quantity using length units, or `nil`.

Note

Provide a total distance value whenever the distance traveled is relevant to the workout type. In addition, add distance samples to a workout using the add(_:to:completion:) method. These samples should sum up to the total distance, while providing detailed information about how the intensity changes over the duration of the workout.

## See Also

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

var totalEnergyBurned: HKQuantity?

The total active energy burned during the workout.

Deprecated

var totalFlightsClimbed: HKQuantity?

The total number of flights of stairs climbed during the workout.

Deprecated

var totalSwimmingStrokeCount: HKQuantity?

The total stroke count for the workout.

Deprecated

