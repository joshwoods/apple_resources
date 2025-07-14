

- HealthKit
- HKWorkoutSessionDelegate
-  workoutSession(\_:didEndActivityWith:date:) 

Instance Method

# workoutSession(\_:didEndActivityWith:date:)

Tells the session that the current workout activity ended.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
optional func workoutSession(
    _ workoutSession: HKWorkoutSession,
    didEndActivityWith workoutConfiguration: HKWorkoutConfiguration,
    date: Date
)
```

## Parameters 

`workoutSession`  

The workout session for the activity that just ended.

`workoutConfiguration`  

The workout configuration object for the activity.

`date`  

The end date and time for the activity.

## See Also

### Tracking workout sessions

func workoutSession(HKWorkoutSession, didChangeTo: HKWorkoutSessionState, from: HKWorkoutSessionState, date: Date)

Tells the delegate that the session’s state changed.

**Required**

func workoutSession(HKWorkoutSession, didFailWithError: any Error)

Tells the delegate that the session failed with an error.

**Required**

func workoutSession(HKWorkoutSession, didGenerate: HKWorkoutEvent)

Tells the delegate that the system generated a workout event.

func workoutSession(HKWorkoutSession, didBeginActivityWith: HKWorkoutConfiguration, date: Date)

Tells the delegate that a new workout session began.

