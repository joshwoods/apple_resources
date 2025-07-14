

- WatchKit
- WKExtendedRuntimeSessionInvalidationReason
-  WKExtendedRuntimeSessionInvalidationReason.suppressedBySystem 

Case

# WKExtendedRuntimeSessionInvalidationReason.suppressedBySystem

The system is in a state that doesn’t allow sessions of this type.

watchOS 6.0+

``` source
case suppressedBySystem
```

## See Also

### Invalidation Reasons

case error

An error prevented the session from running.

case none

The session ended normally.

case sessionInProgress

This app already has a running session.

case expired

The session used all of its allocated time.

case resignedFrontmost

The app lost its frontmost status.

