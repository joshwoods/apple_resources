

- WatchKit
- WKExtendedRuntimeSessionErrorCode
-  WKExtendedRuntimeSessionErrorCode.notYetStarted 

Case

# WKExtendedRuntimeSessionErrorCode.notYetStarted

The app invalidated the session before it started.

watchOS 6.0+

``` source
case notYetStarted
```

## Discussion

The app called the invalidate() method on a session before calling its start() method.

## See Also

### Error Codes

case unknown

An unknown error occurred.

case scheduledTooFarInAdvance

The app attempted to schedule a session too far in the future.

case mustBeActiveToStartOrSchedule

The watchOS app attempted to start or schedule a session while not in an active state.

case exceededResourceLimits

The session exceeded its resource limits.

case barDisabled

The user has disabled background app refresh.

case notApprovedToStartSession

The app attempted to start a session, but doesn’t have a valid session type.

case notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

