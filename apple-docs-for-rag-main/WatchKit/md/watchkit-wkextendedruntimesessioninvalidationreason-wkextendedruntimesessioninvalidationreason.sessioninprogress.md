

- WatchKit
- WKExtendedRuntimeSessionInvalidationReason
-  WKExtendedRuntimeSessionInvalidationReason.sessionInProgress 

Case

# WKExtendedRuntimeSessionInvalidationReason.sessionInProgress

This app already has a running session.

watchOS 6.0+

``` source
case sessionInProgress
```

## Discussion

Each app can only run one extended runtime session at a time.

## See Also

### Invalidation Reasons

case error

An error prevented the session from running.

case none

The session ended normally.

case expired

The session used all of its allocated time.

case resignedFrontmost

The app lost its frontmost status.

case suppressedBySystem

The system is in a state that doesn’t allow sessions of this type.

