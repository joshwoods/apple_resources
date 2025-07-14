

- HealthKit
- HKWorkoutSessionDelegate
-  workoutSession(\_:didGenerate:) 

Instance Method

# workoutSession(\_:didGenerate:)

Tells the delegate that the system generated a workout event.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
optional func workoutSession(
    _ workoutSession: HKWorkoutSession,
    didGenerate event: HKWorkoutEvent
)
```

## Parameters 

`workoutSession`  

The workout session associated with the event.

`event`  

The event that the system generated. For a list of possible values, see HKWorkoutEvent.

## Mentioned in 

Receiving Downhill Skiing and Snowboarding Data

## Discussion

You can save the generated events and use them when creating a HKWorkout object for the session.

## See Also

### Tracking workout sessions

func workoutSession(HKWorkoutSession, didChangeTo: HKWorkoutSessionState, from: HKWorkoutSessionState, date: Date)

Tells the delegate that the session’s state changed.

**Required**

func workoutSession(HKWorkoutSession, didFailWithError: any Error)

Tells the delegate that the session failed with an error.

**Required**

func workoutSession(HKWorkoutSession, didBeginActivityWith: HKWorkoutConfiguration, date: Date)

Tells the delegate that a new workout session began.

func workoutSession(HKWorkoutSession, didEndActivityWith: HKWorkoutConfiguration, date: Date)

Tells the session that the current workout activity ended.

