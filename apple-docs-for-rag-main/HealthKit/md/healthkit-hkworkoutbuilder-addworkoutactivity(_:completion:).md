

- HealthKit
- HKWorkoutBuilder
-  addWorkoutActivity(\_:completion:) 

Instance Method

# addWorkoutActivity(\_:completion:)

Adds a workout activity to the workout builder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func addWorkoutActivity(
    _ workoutActivity: HKWorkoutActivity,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func addWorkoutActivity(_ workoutActivity: HKWorkoutActivity) async throws
```

## Parameters 

`workoutActivity`  

The workout activity to add.

`completion`  

A callback handler that the system calls after adding the workout activity. The system calls the callback handler on an anonymous background queue.

The callback handler takes the following parameters:

success  
Contains true if the builder successfully added the activity.

error  
If the `success` parameter is false, this parameter contains information about the error; otherwise, it’s `nil`.

## Discussion

You can call this method repeatedly to incrementally add activities to the builder. Calling this method after calling finishWorkout(completion:) fails with an error.

If you add an HKWorkoutActivity object that doesn’t have an endDate, you can set the end date by calling updateActivity(uuid:end:completion:).

## See Also

### Managing workout activities

func updateActivity(uuid: UUID, adding: [String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to a workout activity that you’ve already added to the workout builder.

func updateActivity(uuid: UUID, end: Date, completion: (Bool, (any Error)?) -> Void)

Sets the end date for a workout activity that you’ve already added to the workout builder.

var workoutActivities: [HKWorkoutActivity]

