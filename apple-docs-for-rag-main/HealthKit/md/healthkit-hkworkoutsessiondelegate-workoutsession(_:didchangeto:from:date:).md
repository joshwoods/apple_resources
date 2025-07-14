

- HealthKit
- HKWorkoutSessionDelegate
-  workoutSession(\_:didChangeTo:from:date:) 

Instance Method

# workoutSession(\_:didChangeTo:from:date:)

Tells the delegate that the session’s state changed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 10.10+visionOS 1.0+watchOS 2.0+

``` source
func workoutSession(
    _ workoutSession: HKWorkoutSession,
    didChangeTo toState: HKWorkoutSessionState,
    from fromState: HKWorkoutSessionState,
    date: Date
)
```

**Required**

## Parameters 

`workoutSession`  

The workout session that changed.

`toState`  

The session’s new state. For a list of possible values, see HKWorkoutSessionState.

`fromState`  

The session’s previous state. For a list of possible values, see HKWorkoutSessionState.

`date`  

A date object indicating when the state change occurred.

## Discussion

If your application is suspended, the delegate receives this call after the application resumes. This means you may receive the notification long after the state changed. Check the `date` parameter to determine when the state change actually occurred.

For a list of possible session states, see HKWorkoutSessionState.

## See Also

### Tracking workout sessions

func workoutSession(HKWorkoutSession, didFailWithError: any Error)

Tells the delegate that the session failed with an error.

**Required**

func workoutSession(HKWorkoutSession, didGenerate: HKWorkoutEvent)

Tells the delegate that the system generated a workout event.

func workoutSession(HKWorkoutSession, didBeginActivityWith: HKWorkoutConfiguration, date: Date)

Tells the delegate that a new workout session began.

func workoutSession(HKWorkoutSession, didEndActivityWith: HKWorkoutConfiguration, date: Date)

Tells the session that the current workout activity ended.

