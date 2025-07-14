

- WorkoutKit
- SingleGoalWorkout
-  supportsGoal(\_:activity:location:) 

Type Method

# supportsGoal(\_:activity:location:)

Returns a Boolean value that determines whether the system supports the provided goal.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func supportsGoal(
    _ goal: WorkoutGoal,
    activity: HKWorkoutActivityType,
    location: HKWorkoutSessionLocationType = .unknown
) -> Bool
```

## Parameters 

`goal`  

The target goal.

`activity`  

The workout’s activity type.

`location`  

The workout’s location.

## See Also

### Creating single goal workouts

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, swimmingLocation: HKWorkoutSwimmingLocationType, goal: WorkoutGoal)

Creates a new workout with a single goal.

static func supportsActivity(HKWorkoutActivityType) -> Bool

Returns a Boolean value that indicates whether the system supports the provided workout activity.

