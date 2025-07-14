

- WatchKit
- WKExtendedRuntimeSessionErrorCode
-  WKExtendedRuntimeSessionErrorCode.exceededResourceLimits 

Case

# WKExtendedRuntimeSessionErrorCode.exceededResourceLimits

The session exceeded its resource limits.

watchOS 6.0+

``` source
case exceededResourceLimits
```

## Mentioned in 

Using extended runtime sessions

## Discussion

During an extended runtime session, the system limits your app’s amortized CPU usage over time. If your app exceeds the limits during a 60-second window, the system cancels the session. Monitoring usage-per-minute allows your app to experience brief spikes of CPU usage, as long as the average remains low.

When the system cancels your session, it calls your delegate’s extendedRuntimeSession(_:didInvalidateWith:error:) method and passes a WKExtendedRuntimeSessionInvalidationReason.error reason with a WKExtendedRuntimeSessionErrorCode.exceededResourceLimits error.

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

case barDisabled

The user has disabled background app refresh.

case notApprovedToStartSession

The app attempted to start a session, but doesn’t have a valid session type.

case notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

