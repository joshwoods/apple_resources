

- WorkoutKit
-  IntervalBlock 

Structure

# IntervalBlock

Blocks of work and recovery steps that repeat in a custom workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct IntervalBlock
```

## Topics

### Creating an interval block

init(steps: [IntervalStep], iterations: Int)

Creates a new interval block, in which the workout repeats the provided steps the specified number of times.

### Accessing interval block properties

var steps: [IntervalStep]

A series of work and recovery steps for the interval block.

var iterations: Int

The number of times the interval block repeats its steps.

### Hashing interval blocks

var hashValue: Int

The hashed value of the interval block.

func hash(into: inout Hasher)

Hashes the essential components of the interval block by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two interval blocks aren’t equal.

static func == (IntervalBlock, IntervalBlock) -> Bool

Returns a Boolean value that indicates whether two interval blocks are equal.

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

struct IntervalStep

An interval that represents a work or recovery step in a workout.

enum WorkoutGoal

A value that specifies the goal for a workout.

protocol WorkoutAlert

An alert that notifies the user of significant events during a workout.

