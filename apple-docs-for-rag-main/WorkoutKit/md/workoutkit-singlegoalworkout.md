

- WorkoutKit
-  SingleGoalWorkout 

Structure

# SingleGoalWorkout

A workout with a single goal.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct SingleGoalWorkout
```

## Topics

### Creating single goal workouts

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, swimmingLocation: HKWorkoutSwimmingLocationType, goal: WorkoutGoal)

Creates a new workout with a single goal.

static func supportsActivity(HKWorkoutActivityType) -> Bool

Returns a Boolean value that indicates whether the system supports the provided workout activity.

static func supportsGoal(WorkoutGoal, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that determines whether the system supports the provided goal.

### Accessing workout data

var activity: HKWorkoutActivityType

The workout activity type.

var location: HKWorkoutSessionLocationType

The workout location.

var swimmingLocation: HKWorkoutSwimmingLocationType

For swimming workouts, the workout’s swimming location.

var goal: WorkoutGoal

The goal for the workout.

### Comparing workouts

var hashValue: Int

The hashed value of the workout.

func hash(into: inout Hasher)

Hashes the essential components of the workout by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workouts aren’t equal.

static func == (SingleGoalWorkout, SingleGoalWorkout) -> Bool

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

struct PacerWorkout

A workout in which a person covers a specific distance in a given time.

struct SwimBikeRunWorkout

A workout for multisport activities that include running, biking, and swimming.

