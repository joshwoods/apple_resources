

- HealthKit
- HKHealthStore
-  splitTotalEnergy(\_:start:end:resultsHandler:) Deprecated

Instance Method

# splitTotalEnergy(\_:start:end:resultsHandler:)

Calculates the active and resting energy burned based on the total energy burned over the given duration.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
func splitTotalEnergy(
    _ totalEnergy: HKQuantity,
    start startDate: Date,
    end endDate: Date,
    resultsHandler: @escaping (HKQuantity?, HKQuantity?, (any Error)?) -> Void
)
```

Deprecated

No longer supported

## Parameters 

`totalEnergy`  

A quantity object containing the total energy burned during the specified time period.

`startDate`  

A date object representing the activity’s start time.

`endDate`  

A date object representing the activity’s end time.

`resultsHandler`  

A block that is called as soon as the calculations are complete. This block is passed the following parameters:

restingEnergy  
A quantity object containing the resting portion of the total energy.

activeEnergy  
A quantity object containing the active portion of the total energy.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Discussion

This method operates asynchronously. As soon as the calculation is finished, it calls the completion block on a background queue.

This method splits the total calories into the active and resting calories, based on the user’s estimated resting metabolic rate and the activity’s duration. Use the resulting values to create samples representing both the active and resting energy burned.

Active energy samples contribute to Apple Watch’s activity monitoring.

## See Also

### Managing workouts

func recoverActiveWorkoutSession(completion: (HKWorkoutSession?, (any Error)?) -> Void)

Recovers an active workout session.

