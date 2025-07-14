

- WatchKit
- WKExtendedRuntimeSessionInvalidationReason
-  WKExtendedRuntimeSessionInvalidationReason.none 

Case

# WKExtendedRuntimeSessionInvalidationReason.none

The session ended normally.

watchOS 6.0+

``` source
case none
```

## Discussion

The system uses this reason when you stop a session by calling its invalidate() method.

## See Also

### Invalidation Reasons

case error

An error prevented the session from running.

case sessionInProgress

This app already has a running session.

case expired

The session used all of its allocated time.

case resignedFrontmost

The app lost its frontmost status.

case suppressedBySystem

The system is in a state that doesn’t allow sessions of this type.

