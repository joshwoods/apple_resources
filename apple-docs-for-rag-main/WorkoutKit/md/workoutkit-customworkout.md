

- WorkoutKit
-  CustomWorkout 

Structure

# CustomWorkout

A workout that includes a repeating series of work and recovery steps.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct CustomWorkout
```

## Topics

### Creating custom workouts

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, displayName: String?, warmup: WorkoutStep?, blocks: [IntervalBlock], cooldown: WorkoutStep?)

Create a new custom workout.

static func supportsActivity(HKWorkoutActivityType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified workout activity .

static func supportsAlert(WorkoutAlert, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified alert for the given activity type and location.

static func supportsGoal(WorkoutGoal, activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the system supports the specified goal for the given activity type and location.

### Accessing workout data

var displayName: String?

The name that the system uses when displaying the workout.

var activity: HKWorkoutActivityType

The type of activity performed during the workout.

var location: HKWorkoutSessionLocationType

The workout session location for the workout.

var warmup: WorkoutStep?

The warmup step (if any).

var blocks: [IntervalBlock]

A block of repeating work and recovery steps.

var cooldown: WorkoutStep?

The cooldown step (if any).

### Comparing workouts

var hashValue: Int

The hashed value of the custom workout.

func hash(into: inout Hasher)

Hashes the essential components of the custom workout by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two custom workouts aren’t equal.

static func == (CustomWorkout, CustomWorkout) -> Bool

Returns a Boolean value that indicates whether two custom workouts are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Custom interval workouts

struct WorkoutStep

A step in a workout.

struct IntervalBlock

Blocks of work and recovery steps that repeat in a custom workout.

struct IntervalStep

An interval that represents a work or recovery step in a workout.

enum WorkoutGoal

A value that specifies the goal for a workout.

protocol WorkoutAlert

An alert that notifies the user of significant events during a workout.

