

- WorkoutKit
- SwimBikeRunWorkout
-  supportsActivityOrdering(\_:) 

Type Method

# supportsActivityOrdering(\_:)

Returns a Boolean value that indicates whether the system supports a multisport workout with the specified list of activities.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func supportsActivityOrdering(_ activities: [SwimBikeRunWorkout.Activity]) -> Bool
```

## Parameters 

`activities`  

An ordered list of activities for the multisport workout.

## See Also

### Creating new multisport workouts.

init(activities: [SwimBikeRunWorkout.Activity], displayName: String?)

Creates a new multisport workout for the specified activities.

enum Activity

An activity in a multisport workout.

