

- WorkoutKit
- WorkoutPlan
-  WorkoutPlan.Workout 

Enumeration

# WorkoutPlan.Workout

The workout for the workout plan.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
enum Workout
```

## Topics

### Setting the workout

case custom(CustomWorkout)

A custom workout.

case goal(SingleGoalWorkout)

A single goal workout

case pacer(PacerWorkout)

A pacer workout.

case swimBikeRun(SwimBikeRunWorkout)

A multisport workout.

### Accessing workout data

var activity: HKWorkoutActivityType

The workout activity type.

### Comparing workout plans

var hashValue: Int

The hashed value of the workout.

func hash(into: inout Hasher)

Hashes the essential components of the workout by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workouts aren’t equal.

static func == (WorkoutPlan.Workout, WorkoutPlan.Workout) -> Bool

Returns a Boolean value that indicates whether two workouts are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating a workout plan

init(WorkoutPlan.Workout, id: UUID)

Creates a new workout plan from the provided workout and ID.

