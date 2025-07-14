

- AVFoundation
- AVCaptureSession
-  runtimeErrorNotification 

Type Property

# runtimeErrorNotification

A notification the system posts when an error occurs during a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class let runtimeErrorNotification: NSNotification.Name
```

## Discussion

Retrieve the underlying error from the notification’s user information dictionary using the key AVCaptureSessionErrorKey.

## Topics

### User Info Keys

let AVCaptureSessionErrorKey: String

Key to retrieve the error object from a runtimeErrorNotification user info dictionary.

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

class let wasInterruptedNotification: NSNotification.Name

A notification the system posts when it interrupts a capture session.

class let interruptionEndedNotification: NSNotification.Name

A notification the system posts when an interruption to a capture session finishes.

