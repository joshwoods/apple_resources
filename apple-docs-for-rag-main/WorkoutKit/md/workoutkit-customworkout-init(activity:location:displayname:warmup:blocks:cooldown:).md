

- WorkoutKit
- CustomWorkout
-  init(activity:location:displayName:warmup:blocks:cooldown:) 

Initializer

# init(activity:location:displayName:warmup:blocks:cooldown:)

Create a new custom workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(
    activity: HKWorkoutActivityType,
    location: HKWorkoutSessionLocationType = .unknown,
    displayName: String? = nil,
    warmup: WorkoutStep? = nil,
    blocks: [IntervalBlock] = [],
    cooldown: WorkoutStep? = nil
)
```

## Parameters 

`activity`  

The type of activity performed during the workout.

`location`  

The workout session location for the workout.

`displayName`  

The name that the system uses when displaying the workout.

`warmup`  

The warmup step (if any).

`blocks`  

A block of repeating work and recovery steps.

`cooldown`  

The cooldown step (if any).

## See Also

### Creating custom workouts

static func supportsActivity(HKWorkoutActivityType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified workout activity .

static func supportsAlert(WorkoutAlert, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified alert for the given activity type and location.

static func supportsGoal(WorkoutGoal, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified goal for the given activity type and location.

