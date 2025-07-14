

- WatchKit
- WKExtendedRuntimeSessionState
-  WKExtendedRuntimeSessionState.notStarted 

Case

# WKExtendedRuntimeSessionState.notStarted

The app has not yet started or scheduled the session.

watchOS 6.0+

``` source
case notStarted
```

## Discussion

When you instantiate a new session, it stays in the WKExtendedRuntimeSessionState.notStarted state until you call the session’s start() or start(at:) method.

## See Also

### Session States

case scheduled

The app has scheduled the session to run at a future date.

case running

The session is actively running.

case invalid

Either the session has encountered an error, or it has stopped running.

