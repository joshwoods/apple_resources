

- WorkoutKit
-  ScheduledWorkoutPlan 

Structure

# ScheduledWorkoutPlan

A wrapper around a workout plan that your app can use to schedule the workout plan.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct ScheduledWorkoutPlan
```

## Topics

### Creating scheduled workout plans

init(WorkoutPlan, date: DateComponents)

Creates a new scheduled workout plan.

### Accessing plan data

var plan: WorkoutPlan

The target workout plan to schedule.

var date: DateComponents

Date components that determine when the workout should begin.

var complete: Bool

A Boolean value that indicates whether the workout is complete.

### Comparing plans

var hashValue: Int

The hashed value of the scheduled plan.

func hash(into: inout Hasher)

Hashes the essential components of the scheduled plan by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two scheduled plans aren’t equal.

static func == (ScheduledWorkoutPlan, ScheduledWorkoutPlan) -> Bool

Returns a Boolean value that indicates whether two scheduled plans are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Workout plans and schedules

struct WorkoutPlan

A wrapper around a workout object that your app can use to open the object in Workout or schedule it for later.

class WorkoutScheduler

An object for scheduling and managing workouts.

