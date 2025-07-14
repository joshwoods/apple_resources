

- WorkoutKit
-  WorkoutPlan 

Structure

# WorkoutPlan

A wrapper around a workout object that your app can use to open the object in Workout or schedule it for later.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct WorkoutPlan
```

## Topics

### Creating a workout plan

init(WorkoutPlan.Workout, id: UUID)

Creates a new workout plan from the provided workout and ID.

enum Workout

The workout for the workout plan.

### Accessing workout plan data

var id: UUID

A unique identity for the workout plan.

typealias ID

The data type of the workout plan’s ID.

var workout: WorkoutPlan.Workout

The workout represented by this plan.

### Opening the workout plan

func openInWorkoutApp() async throws

Opens the workout in Workout on Apple Watch.

### Initializers

init(from: Data) throws

### Instance Properties

var dataRepresentation: Data

var hashValue: Int

### Instance Methods

func hash(into: inout Hasher)

### Operator Functions

static func != (Self, Self) -> Bool

static func == (WorkoutPlan, WorkoutPlan) -> Bool

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Workout plans and schedules

struct ScheduledWorkoutPlan

A wrapper around a workout plan that your app can use to schedule the workout plan.

class WorkoutScheduler

An object for scheduling and managing workouts.

