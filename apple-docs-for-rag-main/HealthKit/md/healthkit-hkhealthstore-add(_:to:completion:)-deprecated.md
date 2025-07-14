

- HealthKit
- HKHealthStore
-  add(\_:to:completion:) Deprecated

Instance Method

# add(\_:to:completion:)

Associates the provided samples with the specified workout.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.0–16.0DeprecatedmacOS 13.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–10.0Deprecated

``` source
func add(
    _ samples: [HKSample],
    to workout: HKWorkout,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func addSamples(
    _ samples: [HKSample],
    to workout: HKWorkout
) async throws
```

Deprecated

Use HKWorkoutBuilder

## Parameters 

`samples`  

An array containing HKCategorySample or HKQuantitySample objects.

`workout`  

The workout object you are adding samples to.

`completion`  

A block that this method calls as soon as the add-samples operation is complete. This block is passed the following parameters:

success  
A Boolean value. This parameter contains true if the samples were successfully added to workout; otherwise, false.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Mentioned in 

Adding samples to a workout

## Discussion

This method operates asynchronously. As soon as the add-samples operation is finished, this method calls the completion block on a background queue. You must save the workout to the HealthKit store before you can add any samples to it. You can save the samples before calling this method, but doing so is not required. This method automatically saves any unsaved samples when it successfully adds them to the workout.

To query for all the samples associated with a workout, add the workout to the query’s predicate. For example, the query’s predicateForObjects(from:) method creates a predicate object that matches only samples associated with the provided workout.

For more information on workouts and associated samples, see HKWorkout.

## See Also

### Deprecated symbols

func start(HKWorkoutSession)

Starts a workout session for the current app.

Deprecated

func end(HKWorkoutSession)

Ends a workout session for the current app.

Deprecated

