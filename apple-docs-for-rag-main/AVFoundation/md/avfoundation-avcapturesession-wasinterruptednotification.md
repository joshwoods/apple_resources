

- AVFoundation
- AVCaptureSession
-  wasInterruptedNotification 

Type Property

# wasInterruptedNotification

A notification the system posts when it interrupts a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.14+tvOS 17.0+visionOS 1.0+

``` source
class let wasInterruptedNotification: NSNotification.Name
```

## Discussion

Retrieve the underlying error from the notification’s user information dictionary using the key AVCaptureSessionInterruptionReasonKey.

## Topics

### User-Infomation Keys

let AVCaptureSessionInterruptionSystemPressureStateKey: String

A key to retrieve a state value that indicates the system pressure level and contributing factors that caused the interruption.

let AVCaptureSessionInterruptionReasonKey: String

Key to retrieve information about a capture interruption from a wasInterruptedNotification user info dictionary.

enum InterruptionReason

Constants identifying the reason a capture session was interrupted, found in an wasInterruptedNotification user info dictionary.

## See Also

### Observing Session State

var isRunning: Bool

A Boolean value that indicates whether the capture session is in a running state.

var isInterrupted: Bool

A Boolean value that indicates whether the capture session is in an interrupted state.

class let didStartRunningNotification: NSNotification.Name

A notification the system posts when a capture session starts.

class let didStopRunningNotification: NSNotification.Name

A notification the system posts when a capture session stops.

class let interruptionEndedNotification: NSNotification.Name

A notification the system posts when an interruption to a capture session finishes.

class let runtimeErrorNotification: NSNotification.Name

A notification the system posts when an error occurs during a capture session.

