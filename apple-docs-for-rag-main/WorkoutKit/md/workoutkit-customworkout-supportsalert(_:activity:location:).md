

- WorkoutKit
- CustomWorkout
-  supportsAlert(\_:activity:location:) 

Type Method

# supportsAlert(\_:activity:location:)

Returns a Boolean value that indicates whether the system supports the specified alert for the given activity type and location.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

**Mac Catalyst, macOS, watchOS**

``` source
static func supportsAlert(
    _ alert: any WorkoutAlert,
    activity: HKWorkoutActivityType,
    location: HKWorkoutSessionLocationType = .unknown
) -> Bool
```

**iOS, iPadOS**

``` source
static func supportsAlert(
    _ alert: WorkoutAlert,
    activity: HKWorkoutActivityType,
    location: HKWorkoutSessionLocationType = .unknown
) -> Bool
```

## Parameters 

`alert`  

The alert to check.

`activity`  

The workout activity.

`location`  

The workout location.

## See Also

### Creating custom workouts

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, displayName: String?, warmup: WorkoutStep?, blocks: [IntervalBlock], cooldown: WorkoutStep?)

Create a new custom workout.

static func supportsActivity(HKWorkoutActivityType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified workout activity .

static func supportsGoal(WorkoutGoal, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified goal for the given activity type and location.

