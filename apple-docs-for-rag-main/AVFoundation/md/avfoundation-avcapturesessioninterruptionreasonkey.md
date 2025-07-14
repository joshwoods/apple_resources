

- AVFoundation
-  AVCaptureSessionInterruptionReasonKey 

Global Variable

# AVCaptureSessionInterruptionReasonKey

Key to retrieve information about a capture interruption from a wasInterruptedNotification user info dictionary.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
let AVCaptureSessionInterruptionReasonKey: String
```

## Discussion

The value for this key is an NSNumber object containing a AVCaptureSession.InterruptionReason value.

## See Also

### User-Infomation Keys

let AVCaptureSessionInterruptionSystemPressureStateKey: String

A key to retrieve a state value that indicates the system pressure level and contributing factors that caused the interruption.

enum InterruptionReason

Constants identifying the reason a capture session was interrupted, found in an wasInterruptedNotification user info dictionary.

