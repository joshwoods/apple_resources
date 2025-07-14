

- HealthKit
- HKWorkoutSessionState
-  HKWorkoutSessionState.prepared 

Case

# HKWorkoutSessionState.prepared

The session is ready but not yet running.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 5.0+

``` source
case prepared
```

## Discussion

The app can continue to run in the background, even after the user lowers their wrist, but it doesn’t yet generate workout data.

## See Also

### Related Documentation

func prepare()

Prepares the workout session.

### Session states

case notStarted

The workout session has not started.

case running

The workout session is running.

case paused

The workout session has paused.

case stopped

The session has stopped.

case ended

The workout session has ended.

