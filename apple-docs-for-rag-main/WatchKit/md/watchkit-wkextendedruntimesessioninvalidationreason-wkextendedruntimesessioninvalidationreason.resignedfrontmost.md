

- WatchKit
- WKExtendedRuntimeSessionInvalidationReason
-  WKExtendedRuntimeSessionInvalidationReason.resignedFrontmost 

Case

# WKExtendedRuntimeSessionInvalidationReason.resignedFrontmost

The app lost its frontmost status.

watchOS 6.0+

``` source
case resignedFrontmost
```

## Discussion

If the session type doesn’t grant background execution time, the session stops as soon as the app loses its frontmost app status. Users can dismiss the frontmost app by pressing the Digital Crown, tapping a notification, or launching another app. For more information, see `Understand Frontmost App State`.

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

case suppressedBySystem

The system is in a state that doesn’t allow sessions of this type.

