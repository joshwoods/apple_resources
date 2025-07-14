

- WorkoutKit
-  WorkoutStep 

Structure

# WorkoutStep

A step in a workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct WorkoutStep
```

## Topics

### Creating new workout steps

init(goal: WorkoutGoal, alert: (WorkoutAlert)?)

Creates a new workout step with the provided goal and alerts.

### Accessing step data

var alert: (WorkoutAlert)?

Alerts used during the step.

var goal: WorkoutGoal

A goal that determines when the step ends.

### Comparing workout steps

var hashValue: Int

The hashed value of the workout step.

func hash(into: inout Hasher)

Hashes the essential components of the workout step by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workout steps aren’t equal.

static func == (WorkoutStep, WorkoutStep) -> Bool

Returns a Boolean value that indicates whether two workout steps are equal.

### Initializers

init(goal: WorkoutGoal, alert: (any WorkoutAlert)?, displayName: String?)

### Instance Properties

var displayName: String?

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

struct IntervalBlock

Blocks of work and recovery steps that repeat in a custom workout.

struct IntervalStep

An interval that represents a work or recovery step in a workout.

enum WorkoutGoal

A value that specifies the goal for a workout.

protocol WorkoutAlert

An alert that notifies the user of significant events during a workout.

