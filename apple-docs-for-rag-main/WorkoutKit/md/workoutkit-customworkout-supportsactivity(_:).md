

- WorkoutKit
- CustomWorkout
-  supportsActivity(\_:) 

Type Method

# supportsActivity(\_:)

Returns a Boolean value that indicates whether the system supports the specified workout activity .

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func supportsActivity(_ activity: HKWorkoutActivityType) -> Bool
```

## Parameters 

`activity`  

The activity to check.

## See Also

### Creating custom workouts

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, displayName: String?, warmup: WorkoutStep?, blocks: [IntervalBlock], cooldown: WorkoutStep?)

Create a new custom workout.

static func supportsAlert(WorkoutAlert, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified alert for the given activity type and location.

static func supportsGoal(WorkoutGoal, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified goal for the given activity type and location.

