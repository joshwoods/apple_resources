

- HealthKit
- HKWorkoutSessionState
-  HKWorkoutSessionState.stopped 

Case

# HKWorkoutSessionState.stopped

The session has stopped.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 5.0+

``` source
case stopped
```

## Discussion

As soon as the session stops, the watch’s sensors return to normal, and it no longer generates workout data; however, the app can continue to run in the background, even after the user lowers their wrist.

You can’t restart or reuse the workout session.

## See Also

### Session states

case notStarted

The workout session has not started.

case prepared

The session is ready but not yet running.

case running

The workout session is running.

case paused

The workout session has paused.

case ended

The workout session has ended.

