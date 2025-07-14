

- WorkoutKit
- WorkoutScheduler
-  scheduledWorkouts 

Instance Property

# scheduledWorkouts

An array of all the workouts scheduled by your app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
final var scheduledWorkouts: [ScheduledWorkoutPlan] { get async }
```

## See Also

### Managing scheduled workouts

static let maxAllowedScheduledWorkoutCount: Int

The maximum number of workouts your app can schedule.

func markComplete(WorkoutPlan, at: DateComponents) async

Marks the workout as complete.

func remove(WorkoutPlan, at: DateComponents) async

Removes the scheduled workout.

func removeAllWorkouts() async

Removes all scheduled workouts.

