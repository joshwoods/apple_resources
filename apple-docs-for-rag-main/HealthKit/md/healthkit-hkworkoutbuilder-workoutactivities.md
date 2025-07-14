

- HealthKit
- HKWorkoutBuilder
-  workoutActivities 

Instance Property

# workoutActivities

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var workoutActivities: [HKWorkoutActivity] { get }
```

## See Also

### Managing workout activities

func addWorkoutActivity(HKWorkoutActivity, completion: (Bool, (any Error)?) -> Void)

Adds a workout activity to the workout builder.

func updateActivity(uuid: UUID, adding: [String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to a workout activity that you’ve already added to the workout builder.

func updateActivity(uuid: UUID, end: Date, completion: (Bool, (any Error)?) -> Void)

Sets the end date for a workout activity that you’ve already added to the workout builder.

