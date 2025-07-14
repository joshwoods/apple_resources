

- HealthKit
- HKWorkoutSessionDelegate
-  workoutSession(\_:didFailWithError:) 

Instance Method

# workoutSession(\_:didFailWithError:)

Tells the delegate that the session failed with an error.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
func workoutSession(
    _ workoutSession: HKWorkoutSession,
    didFailWithError error: any Error
)
```

**Required**

## Parameters 

`workoutSession`  

The workout session that failed.

`error`  

An error object describing the failure.

## Discussion

When the state of the workout session changes due to an error, HealthKit always calls this method before calling the workoutSession(_:didChangeTo:from:date:) method.

For example, if a second app starts a workout session, HealthKit calls the current session’s workoutSession(_:didFailWithError:) method. Next, it changes current session’s state to the HKWorkoutSessionState.ended value. Finally, HealthKit calls the current session’s workoutSession(_:didChangeTo:from:date:) method.

## See Also

### Tracking workout sessions

func workoutSession(HKWorkoutSession, didChangeTo: HKWorkoutSessionState, from: HKWorkoutSessionState, date: Date)

Tells the delegate that the session’s state changed.

**Required**

func workoutSession(HKWorkoutSession, didGenerate: HKWorkoutEvent)

Tells the delegate that the system generated a workout event.

func workoutSession(HKWorkoutSession, didBeginActivityWith: HKWorkoutConfiguration, date: Date)

Tells the delegate that a new workout session began.

func workoutSession(HKWorkoutSession, didEndActivityWith: HKWorkoutConfiguration, date: Date)

Tells the session that the current workout activity ended.

