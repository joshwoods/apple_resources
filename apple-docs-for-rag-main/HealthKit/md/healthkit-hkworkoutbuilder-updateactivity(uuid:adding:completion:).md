

- HealthKit
- HKWorkoutBuilder
-  updateActivity(uuid:adding:completion:) 

Instance Method

# updateActivity(uuid:adding:completion:)

Adds metadata to a workout activity that you’ve already added to the workout builder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func updateActivity(
    uuid UUID: UUID,
    adding metadata: [String : Any],
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func updateActivity(
    uuid UUID: UUID,
    adding metadata: [String : Any]
) async throws
```

## Parameters 

`UUID`  

The workout activity’s universally unique identifier (UUID).

`metadata`  

A dictionary containing the metadata keys and values to add to the workout activity.

`completion`  

A callback handler that the system calls after updating the workout activity. The system calls the callback handler on an anonymous background queue.

The callback handler takes the following parameters:

success  
Contains true if the builder successfully updates the activity.

error  
If the `success` parameter is false, this parameter contains information about the error; otherwise, it’s `nil`.

## Discussion

You can call this method multiple times to incrementally add metadata to the workout activity. The system merges the new metadata with any existing metadata using addEntriesFromDictionary:. Calling this method after calling finishWorkout(completion:) fails with an error.

## See Also

### Managing workout activities

func addWorkoutActivity(HKWorkoutActivity, completion: (Bool, (any Error)?) -> Void)

Adds a workout activity to the workout builder.

func updateActivity(uuid: UUID, end: Date, completion: (Bool, (any Error)?) -> Void)

Sets the end date for a workout activity that you’ve already added to the workout builder.

var workoutActivities: [HKWorkoutActivity]

