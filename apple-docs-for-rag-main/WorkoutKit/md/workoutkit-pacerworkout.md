

- WorkoutKit
-  PacerWorkout 

Structure

# PacerWorkout

A workout in which a person covers a specific distance in a given time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct PacerWorkout
```

## Topics

### Creating a new pacer workout

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, distance: Measurement&lt;UnitLength>, time: Measurement&lt;UnitDuration>)

Creates a new pacer workout for the specified distance and time.

static func supportsActivity(HKWorkoutActivityType) -> Bool

Returns a Boolean value that indicates whether the system supports pacer workouts for the given workout activity type.

### Accessing workout data

var activity: HKWorkoutActivityType

The workout activity type.

var location: HKWorkoutSessionLocationType

The workout location.

var distance: Measurement&lt;UnitLength>

A length measurement representing the distance goal.

var time: Measurement&lt;UnitDuration>

A time measurement representing the time goal.

### Comparing workouts

var hashValue: Int

The hashed value of the workout.

func hash(into: inout Hasher)

Hashes the essential components of the workout by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workouts aren’t equal.

static func == (PacerWorkout, PacerWorkout) -> Bool

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

struct SwimBikeRunWorkout

A workout for multisport activities that include running, biking, and swimming.

