

- HealthKit
- HKWorkoutSession
-  endCurrentActivity(on:) 

Instance Method

# endCurrentActivity(on:)

Ends the current workout activity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 9.0+

``` source
func endCurrentActivity(on date: Date)
```

## Parameters 

`date`  

The end date and time for the activity.

## Mentioned in 

Dividing a HealthKit workout into activities

## Discussion

This method asynchronously ends the current activity. HealthKit calls the session delegate’s workoutSession(_:didEndActivityWith:date:) method after the activity ends. HealthKit stops collecting data related to this activity.

## See Also

### Managing workout activities

var currentActivity: HKWorkoutActivity

The current workout activity.

func beginNewActivity(configuration: HKWorkoutConfiguration, date: Date, metadata: [String : Any]?)

Begins a new workout activity in the workout session.

