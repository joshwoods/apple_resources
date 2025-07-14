

- HealthKit
- HKWorkout
-  workoutEvents 

Instance Property

# workoutEvents

An array of workout event objects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var workoutEvents: [HKWorkoutEvent]? { get }
```

## Discussion

This array specifies when the user has paused and resumed the workout activity. This method calculates the workout’s duration based on the amount of active time between the provided start and end dates. For more information on workout events, see HKWorkoutEvent.

## See Also

### Accessing workout data

var duration: TimeInterval

The workout’s duration.

var workoutActivityType: HKWorkoutActivityType

The type of activity performed during the workout.

var workoutActivities: [HKWorkoutActivity]

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

