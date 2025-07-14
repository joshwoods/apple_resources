

- WatchKit
- WKExtendedRuntimeSessionErrorCode
-  WKExtendedRuntimeSessionErrorCode.notApprovedToSchedule 

Case

# WKExtendedRuntimeSessionErrorCode.notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

watchOS 6.0+

``` source
case notApprovedToSchedule
```

## Discussion

You can schedule alarm sessions by calling the session’s start(at:) method. For all other session types, use the start() method instead.

## See Also

### Error Codes

case unknown

An unknown error occurred.

case scheduledTooFarInAdvance

The app attempted to schedule a session too far in the future.

case mustBeActiveToStartOrSchedule

The watchOS app attempted to start or schedule a session while not in an active state.

case notYetStarted

The app invalidated the session before it started.

case exceededResourceLimits

The session exceeded its resource limits.

case barDisabled

The user has disabled background app refresh.

case notApprovedToStartSession

The app attempted to start a session, but doesn’t have a valid session type.

