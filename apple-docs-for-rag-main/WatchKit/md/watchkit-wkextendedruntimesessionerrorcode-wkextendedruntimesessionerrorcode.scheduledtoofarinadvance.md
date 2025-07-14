

- WatchKit
- WKExtendedRuntimeSessionErrorCode
-  WKExtendedRuntimeSessionErrorCode.scheduledTooFarInAdvance 

Case

# WKExtendedRuntimeSessionErrorCode.scheduledTooFarInAdvance

The app attempted to schedule a session too far in the future.

watchOS 6.0+

``` source
case scheduledTooFarInAdvance
```

## Discussion

You can’t schedule alarm sessions more than 36 hours in advance. Other session types do not support scheduling.

## See Also

### Error Codes

case unknown

An unknown error occurred.

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

case notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

