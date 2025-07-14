

- WorkoutKit
- SwimBikeRunWorkout
-  SwimBikeRunWorkout.Activity 

Enumeration

# SwimBikeRunWorkout.Activity

An activity in a multisport workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
enum Activity
```

## Topics

### Setting valid activities

case cycling(HKWorkoutSessionLocationType)

A cycling workout activity, with the specified location type.

case running(HKWorkoutSessionLocationType)

A running workout activity, with the specified location type.

case swimming(HKWorkoutSwimmingLocationType)

A swimming workout activity, with the specified location type.

### Comparing activities

var hashValue: Int

The hashed value of the activity.

func hash(into: inout Hasher)

Hashes the essential components of the activity by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two activities aren’t equal.

static func == (SwimBikeRunWorkout.Activity, SwimBikeRunWorkout.Activity) -> Bool

Returns a Boolean value that indicates whether two activities are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating new multisport workouts.

init(activities: [SwimBikeRunWorkout.Activity], displayName: String?)

Creates a new multisport workout for the specified activities.

static func supportsActivityOrdering([SwimBikeRunWorkout.Activity]) -> Bool

Returns a Boolean value that indicates whether the system supports a multisport workout with the specified list of activities.

