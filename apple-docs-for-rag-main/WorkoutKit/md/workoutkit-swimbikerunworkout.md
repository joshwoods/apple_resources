

- WorkoutKit
-  SwimBikeRunWorkout 

Structure

# SwimBikeRunWorkout

A workout for multisport activities that include running, biking, and swimming.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct SwimBikeRunWorkout
```

## Topics

### Creating new multisport workouts.

init(activities: [SwimBikeRunWorkout.Activity], displayName: String?)

Creates a new multisport workout for the specified activities.

enum Activity

An activity in a multisport workout.

static func supportsActivityOrdering([SwimBikeRunWorkout.Activity]) -> Bool

Returns a Boolean value that indicates whether the system supports a multisport workout with the specified list of activities.

### Accessing workout data

var activities: [SwimBikeRunWorkout.Activity]

An ordered list of activities for the multisport workout.

var displayName: String?

The name that the system uses when displaying the workout.

### Comparing workouts

var hashValue: Int

The hashed value of the workout.

func hash(into: inout Hasher)

Hashes the essential components of the workout by feeding them into the given hash function.

static func == (SwimBikeRunWorkout, SwimBikeRunWorkout) -> Bool

Returns a Boolean value that indicates whether two workouts aren’t equal.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workouts are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Common workouts

struct SingleGoalWorkout

A workout with a single goal.

struct PacerWorkout

A workout in which a person covers a specific distance in a given time.

