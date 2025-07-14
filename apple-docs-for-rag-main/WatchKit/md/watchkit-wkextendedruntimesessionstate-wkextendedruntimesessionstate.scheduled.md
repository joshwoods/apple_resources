

- WatchKit
- WKExtendedRuntimeSessionState
-  WKExtendedRuntimeSessionState.scheduled 

Case

# WKExtendedRuntimeSessionState.scheduled

The app has scheduled the session to run at a future date.

watchOS 6.0+

``` source
case scheduled
```

## Discussion

The session transitions to the WKExtendedRuntimeSessionState.scheduled state when you call the start(at:) method. It remains in this state until the start date arrives. Then it transitions to the running state.

## See Also

### Session States

case notStarted

The app has not yet started or scheduled the session.

case running

The session is actively running.

case invalid

Either the session has encountered an error, or it has stopped running.

