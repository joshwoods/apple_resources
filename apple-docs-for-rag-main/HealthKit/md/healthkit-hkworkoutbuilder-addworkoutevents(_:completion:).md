

- HealthKit
- HKWorkoutBuilder
-  addWorkoutEvents(\_:completion:) 

Instance Method

# addWorkoutEvents(\_:completion:)

Adds a workout event to the builder.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func addWorkoutEvents(
    _ workoutEvents: [HKWorkoutEvent],
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func addWorkoutEvents(_ workoutEvents: [HKWorkoutEvent]) async throws
```

## Mentioned in 

Running workout sessions

## See Also

### Adding events to the workout

var workoutEvents: [HKWorkoutEvent]

The list of events added to the workout.

