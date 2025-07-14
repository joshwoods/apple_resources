

- WatchKit
- WKExtendedRuntimeSessionState
-  WKExtendedRuntimeSessionState.invalid 

Case

# WKExtendedRuntimeSessionState.invalid

Either the session has encountered an error, or it has stopped running.

watchOS 6.0+

``` source
case invalid
```

## Discussion

The system passes a WKExtendedRuntimeSessionInvalidationReason value to the session delegate’s extendedRuntimeSession(_:didInvalidateWith:error:) method. Use this value to determine why the session became invalid.

## See Also

### Session States

case notStarted

The app has not yet started or scheduled the session.

case scheduled

The app has scheduled the session to run at a future date.

case running

The session is actively running.

