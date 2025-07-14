

- WorkoutKit
- SingleGoalWorkout
-  init(activity:location:swimmingLocation:goal:) 

Initializer

# init(activity:location:swimmingLocation:goal:)

Creates a new workout with a single goal.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(
    activity: HKWorkoutActivityType,
    location: HKWorkoutSessionLocationType = .unknown,
    swimmingLocation: HKWorkoutSwimmingLocationType = .unknown,
    goal: WorkoutGoal = .open
)
```

## Parameters 

`activity`  

The workout activity type.

`location`  

The workout location.

`swimmingLocation`  

For swimming workouts, the workout’s swimming location.

`goal`  

The goal for the workout.

## See Also

### Creating single goal workouts

static func supportsActivity(HKWorkoutActivityType) -> Bool

Returns a Boolean value that indicates whether the system supports the provided workout activity.

static func supportsGoal(WorkoutGoal, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that determines whether the system supports the provided goal.

