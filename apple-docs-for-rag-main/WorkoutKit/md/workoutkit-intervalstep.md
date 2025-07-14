

- WorkoutKit
-  IntervalStep 

Structure

# IntervalStep

An interval that represents a work or recovery step in a workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct IntervalStep
```

## Topics

### Creating interval steps

init(IntervalStep.Purpose, goal: WorkoutGoal, alert: (WorkoutAlert)?)

init(IntervalStep.Purpose, step: WorkoutStep)

Creates a new interval step.

### Accessing step data

var purpose: IntervalStep.Purpose

The purpose of the interval step.

var step: WorkoutStep

The workout step to perform.

### Comparing interval steps

var hashValue: Int

The hashed value of the interval step.

func hash(into: inout Hasher)

Hashes the essential components of the interval step by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two interval steps aren’t equal.

static func == (IntervalStep, IntervalStep) -> Bool

Returns a Boolean value that indicates whether two interval steps are equal.

### Enumerations

enum Purpose

An interval step’s purpose.

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

enum WorkoutGoal

A value that specifies the goal for a workout.

protocol WorkoutAlert

An alert that notifies the user of significant events during a workout.

