

- HealthKit
- HKWorkout
-  workoutActivityType 

Instance Property

# workoutActivityType

The type of activity performed during the workout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var workoutActivityType: HKWorkoutActivityType { get }
```

## Discussion

For the complete list of activity types, see HKWorkoutActivityType.

## See Also

### Accessing workout data

var duration: TimeInterval

The workout’s duration.

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

var totalSwimmingStrokeCount: HKQuantity?

The total stroke count for the workout.

Deprecated

