

- WorkoutKit
- CustomWorkout
-  location 

Instance Property

# location

The workout session location for the workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
var location: HKWorkoutSessionLocationType { get set }
```

## See Also

### Accessing workout data

var displayName: String?

The name that the system uses when displaying the workout.

var activity: HKWorkoutActivityType

The type of activity performed during the workout.

var warmup: WorkoutStep?

The warmup step (if any).

var blocks: [IntervalBlock]

A block of repeating work and recovery steps.

var cooldown: WorkoutStep?

The cooldown step (if any).

