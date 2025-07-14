

- WatchKit
- WKExtendedRuntimeSessionErrorCode
-  WKExtendedRuntimeSessionErrorCode.barDisabled 

Case

# WKExtendedRuntimeSessionErrorCode.barDisabled

The user has disabled background app refresh.

watchOS 6.0+

``` source
case barDisabled
```

## Discussion

If the user has disabled Background App Refresh for this app, any attempt to schedule a session by calling the start(at:) method fails. The system calls your delegate’s extendedRuntimeSession(_:didInvalidateWith:error:) method and passes a WKExtendedRuntimeSessionInvalidationReason.error reason with a WKExtendedRuntimeSessionErrorCode.barDisabled error.

Users can turn off Background App Refresh by selecting General \> Background App Refresh in the Watch App.

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

case notApprovedToStartSession

The app attempted to start a session, but doesn’t have a valid session type.

case notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

