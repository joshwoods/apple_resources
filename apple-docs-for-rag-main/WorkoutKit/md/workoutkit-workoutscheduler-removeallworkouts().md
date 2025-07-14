

- WorkoutKit
- WorkoutScheduler
-  removeAllWorkouts() 

Instance Method

# removeAllWorkouts()

Removes all scheduled workouts.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
final func removeAllWorkouts() async
```

## See Also

### Managing scheduled workouts

var scheduledWorkouts: [ScheduledWorkoutPlan]

An array of all the workouts scheduled by your app.

static let maxAllowedScheduledWorkoutCount: Int

The maximum number of workouts your app can schedule.

func markComplete(WorkoutPlan, at: DateComponents) async

Marks the workout as complete.

func remove(WorkoutPlan, at: DateComponents) async

Removes the scheduled workout.

