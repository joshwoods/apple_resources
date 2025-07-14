

- HealthKit
- HKWorkoutBuilder
-  workoutEvents 

Instance Property

# workoutEvents

The list of events added to the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
var workoutEvents: [HKWorkoutEvent] { get }
```

## Mentioned in 

Running workout sessions

## See Also

### Adding events to the workout

func addWorkoutEvents([HKWorkoutEvent], completion: (Bool, (any Error)?) -> Void)

Adds a workout event to the builder.

