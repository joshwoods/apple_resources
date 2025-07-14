

- WorkoutKit
-  WorkoutScheduler 

Class

# WorkoutScheduler

An object for scheduling and managing workouts.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
final class WorkoutScheduler
```

## Topics

### Accessing the scheduler

static let shared: WorkoutScheduler

A shared instance of the workout scheduler.

static var isSupported: Bool

A Boolean value that indicates whether the current device supports scheduled workouts.

func requestAuthorization() async -> WorkoutScheduler.AuthorizationState

Requests authorization to schedule workouts.

var authorizationState: WorkoutScheduler.AuthorizationState

The workout scheduler’s authorization status.

enum AuthorizationState

The workout scheduler’s authorization status.

### Scheduling workouts

func schedule(WorkoutPlan, at: DateComponents) async

Schedules the provided workout at the specified date.

### Managing scheduled workouts

var scheduledWorkouts: [ScheduledWorkoutPlan]

An array of all the workouts scheduled by your app.

static let maxAllowedScheduledWorkoutCount: Int

The maximum number of workouts your app can schedule.

func markComplete(WorkoutPlan, at: DateComponents) async

Marks the workout as complete.

func remove(WorkoutPlan, at: DateComponents) async

Removes the scheduled workout.

func removeAllWorkouts() async

Removes all scheduled workouts.

## See Also

### Workout plans and schedules

struct WorkoutPlan

A wrapper around a workout object that your app can use to open the object in Workout or schedule it for later.

struct ScheduledWorkoutPlan

A wrapper around a workout plan that your app can use to schedule the workout plan.

