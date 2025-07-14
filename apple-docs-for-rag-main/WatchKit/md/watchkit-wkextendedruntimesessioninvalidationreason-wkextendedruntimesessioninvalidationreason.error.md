

- WatchKit
- WKExtendedRuntimeSessionInvalidationReason
-  WKExtendedRuntimeSessionInvalidationReason.error 

Case

# WKExtendedRuntimeSessionInvalidationReason.error

An error prevented the session from running.

watchOS 6.0+

``` source
case error
```

## Discussion

When the system passes this value to your extension delegate’s extendedRuntimeSession(_:didInvalidateWith:error:) method, check the `error` parameter for additional information about the error.

## See Also

### Invalidation Reasons

case none

The session ended normally.

case sessionInProgress

This app already has a running session.

case expired

The session used all of its allocated time.

case resignedFrontmost

The app lost its frontmost status.

case suppressedBySystem

The system is in a state that doesn’t allow sessions of this type.

