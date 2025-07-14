

- WorkoutKit
- SingleGoalWorkout
-  supportsActivity(\_:) 

Type Method

# supportsActivity(\_:)

Returns a Boolean value that indicates whether the system supports the provided workout activity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func supportsActivity(_ activity: HKWorkoutActivityType) -> Bool
```

## Parameters 

`activity`  

The target workout activity type.

## See Also

### Creating single goal workouts

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, swimmingLocation: HKWorkoutSwimmingLocationType, goal: WorkoutGoal)

Creates a new workout with a single goal.

static func supportsGoal(WorkoutGoal, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that determines whether the system supports the provided goal.

