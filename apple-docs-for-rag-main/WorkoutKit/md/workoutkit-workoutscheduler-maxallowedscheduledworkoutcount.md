

- WorkoutKit
- WorkoutScheduler
-  maxAllowedScheduledWorkoutCount 

Type Property

# maxAllowedScheduledWorkoutCount

The maximum number of workouts your app can schedule.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static let maxAllowedScheduledWorkoutCount: Int
```

## See Also

### Managing scheduled workouts

var scheduledWorkouts: [ScheduledWorkoutPlan]

An array of all the workouts scheduled by your app.

func markComplete(WorkoutPlan, at: DateComponents) async

Marks the workout as complete.

func remove(WorkoutPlan, at: DateComponents) async

Removes the scheduled workout.

func removeAllWorkouts() async

Removes all scheduled workouts.

