

- WatchKit
- WKExtendedRuntimeSessionInvalidationReason
-  WKExtendedRuntimeSessionInvalidationReason.expired 

Case

# WKExtendedRuntimeSessionInvalidationReason.expired

The session used all of its allocated time.

watchOS 6.0+

``` source
case expired
```

## Discussion

Sessions can only run for a limited amount of time. Each session type has a different time limit. For more information, see the session’s expirationDate property.

## See Also

### Invalidation Reasons

case error

An error prevented the session from running.

case none

The session ended normally.

case sessionInProgress

This app already has a running session.

case resignedFrontmost

The app lost its frontmost status.

case suppressedBySystem

The system is in a state that doesn’t allow sessions of this type.

