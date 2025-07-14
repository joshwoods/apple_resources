

- HealthKit
- HKWorkoutSessionState
-  HKWorkoutSessionState.ended 

Case

# HKWorkoutSessionState.ended

The workout session has ended.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
case ended
```

## Discussion

The watch can no longer run in the background. Its sensors return to normal, and it no longer generates workout data. You can’t restart or reuse the workout session.

## See Also

### Related Documentation

func end()

Ends the workout session.

### Session states

case notStarted

The workout session has not started.

case prepared

The session is ready but not yet running.

case running

The workout session is running.

case paused

The workout session has paused.

case stopped

The session has stopped.

