

- HealthKit
- HKWorkoutBuilder
-  updateActivity(uuid:end:completion:) 

Instance Method

# updateActivity(uuid:end:completion:)

Sets the end date for a workout activity that you’ve already added to the workout builder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func updateActivity(
    uuid UUID: UUID,
    end endDate: Date,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func updateActivity(
    uuid UUID: UUID,
    end endDate: Date
) async throws
```

## Parameters 

`UUID`  

The workout activity’s universally unique identifier (UUID).

`endDate`  

The end date and time for the workout activity.

`completion`  

A callback handler that the system calls after updating the workout activity. The system calls the callback handler on an anonymous background queue.

The callback handler takes the following parameters:

success  
Contains true if the builder successfully updates the activity.

error  
If the `success` parameter is false, this parameter contains information about the error; otherwise, it’s `nil`.

## Discussion

Calling this method after calling finishWorkout(completion:) fails with an error.

## See Also

### Managing workout activities

func addWorkoutActivity(HKWorkoutActivity, completion: (Bool, (any Error)?) -> Void)

Adds a workout activity to the workout builder.

func updateActivity(uuid: UUID, adding: [String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to a workout activity that you’ve already added to the workout builder.

var workoutActivities: [HKWorkoutActivity]

