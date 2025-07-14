

- WatchKit
- WKExtendedRuntimeSessionErrorCode
-  WKExtendedRuntimeSessionErrorCode.mustBeActiveToStartOrSchedule 

Case

# WKExtendedRuntimeSessionErrorCode.mustBeActiveToStartOrSchedule

The watchOS app attempted to start or schedule a session while not in an active state.

watchOS 6.0+

``` source
case mustBeActiveToStartOrSchedule
```

## Discussion

You can only start or schedule sessions when the watchOS app is running in the foreground. Specifically, the WatchKit extension’s applicationState must equal WKApplicationState.active.

## See Also

### Error Codes

case unknown

An unknown error occurred.

case scheduledTooFarInAdvance

The app attempted to schedule a session too far in the future.

case notYetStarted

The app invalidated the session before it started.

case exceededResourceLimits

The session exceeded its resource limits.

case barDisabled

The user has disabled background app refresh.

case notApprovedToStartSession

The app attempted to start a session, but doesn’t have a valid session type.

case notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

