

- WatchKit
- WKExtendedRuntimeSessionErrorCode
-  WKExtendedRuntimeSessionErrorCode.notApprovedToStartSession 

Case

# WKExtendedRuntimeSessionErrorCode.notApprovedToStartSession

The app attempted to start a session, but doesn’t have a valid session type.

watchOS 6.0+

``` source
case notApprovedToStartSession
```

## Discussion

To use extended runtime sessions, your app must enable the Background Mode capability and select a session type.

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

case notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

