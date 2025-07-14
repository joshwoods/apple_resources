

- HealthKit
- HKWorkout
-  duration 

Instance Property

# duration

The workout’s duration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var duration: TimeInterval { get }
```

## Mentioned in 

Adding samples to a workout

## Discussion

A workout’s duration can be specified in one of three ways. The init(activityType:start:end:) method uses the time interval between the provided start and end dates. The init(activityType:start:end:duration:totalEnergyBurned:totalDistance:metadata:) method sets the duration to the provided value. And the init(activityType:start:end:workoutEvents:totalEnergyBurned:totalDistance:metadata:) method calculates the total active duration based on the start and end dates and the workout events.

## See Also

### Accessing workout data

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

var totalSwimmingStrokeCount: HKQuantity?

The total stroke count for the workout.

Deprecated

