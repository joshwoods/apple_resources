

- WorkoutKit
- SwimBikeRunWorkout
-  init(activities:displayName:) 

Initializer

# init(activities:displayName:)

Creates a new multisport workout for the specified activities.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(
    activities: [SwimBikeRunWorkout.Activity],
    displayName: String? = nil
)
```

## Parameters 

`activities`  

An ordered list of workout activity types included in the workout.

`displayName`  

The name that the system uses when displaying the workout.

## See Also

### Creating new multisport workouts.

enum Activity

An activity in a multisport workout.

static func supportsActivityOrdering([SwimBikeRunWorkout.Activity]) -> Bool

Returns a Boolean value that indicates whether the system supports a multisport workout with the specified list of activities.

