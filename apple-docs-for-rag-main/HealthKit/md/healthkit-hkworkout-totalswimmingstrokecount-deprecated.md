

- HealthKit
- HKWorkout
-  totalSwimmingStrokeCount Deprecated

Instance Property

# totalSwimmingStrokeCount

The total stroke count for the workout.

iOS 10.0–18.0DeprecatediPadOS 10.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 3.0–11.0Deprecated

``` source
var totalSwimmingStrokeCount: HKQuantity? { get }
```

Deprecated

Use allStatistics or statistics(for:) instead.

## Discussion

This property contains a quantity using count units, or `nil`.

Note

Provide a total stroke count value whenever the stroke count is relevant to the workout type. In addition, add stroke count samples to a workout using the add(_:to:completion:) method. These samples should sum up to the total stroke count, while providing detailed information about how the intensity changes over the duration of the workout.

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

var totalDistance: HKQuantity?

The total distance traveled during the workout.

Deprecated

var totalEnergyBurned: HKQuantity?

The total active energy burned during the workout.

Deprecated

var totalFlightsClimbed: HKQuantity?

The total number of flights of stairs climbed during the workout.

Deprecated

