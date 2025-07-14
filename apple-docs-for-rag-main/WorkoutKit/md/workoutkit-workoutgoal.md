

- WorkoutKit
-  WorkoutGoal 

Enumeration

# WorkoutGoal

A value that specifies the goal for a workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
enum WorkoutGoal
```

## Topics

### Determining workout goals

case open

An open workout with no set goal.

case distance(Double, UnitLength)

A goal based on distance traveled during the workout.

case energy(Double, UnitEnergy)

A goal based on the amount of energy burned during the workout.

case time(Double, UnitDuration)

A goal based on the amount of time that has elapsed during the workout.

### Comparing workout goals

var hashValue: Int

The hashed value of the workout goal.

func hash(into: inout Hasher)

Hashes the essential components of the workout goal by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workout goals aren’t equal.

static func == (WorkoutGoal, WorkoutGoal) -> Bool

Returns a Boolean value that indicates whether two workout goals are equal.

### Enumeration Cases

case poolSwimDistanceWithTime(Measurement&lt;UnitLength>, Measurement&lt;UnitDuration>)

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Custom interval workouts

struct CustomWorkout

A workout that includes a repeating series of work and recovery steps.

struct WorkoutStep

A step in a workout.

struct IntervalBlock

Blocks of work and recovery steps that repeat in a custom workout.

struct IntervalStep

An interval that represents a work or recovery step in a workout.

protocol WorkoutAlert

An alert that notifies the user of significant events during a workout.

