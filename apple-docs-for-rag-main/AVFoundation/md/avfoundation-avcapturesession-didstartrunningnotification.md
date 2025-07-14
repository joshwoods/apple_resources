

- AVFoundation
- AVCaptureSession
-  didStartRunningNotification 

Type Property

# didStartRunningNotification

A notification the system posts when a capture session starts.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class let didStartRunningNotification: NSNotification.Name
```

## See Also

### Observing Session State

var isRunning: Bool

A Boolean value that indicates whether the capture session is in a running state.

var isInterrupted: Bool

A Boolean value that indicates whether the capture session is in an interrupted state.

class let didStopRunningNotification: NSNotification.Name

A notification the system posts when a capture session stops.

class let wasInterruptedNotification: NSNotification.Name

A notification the system posts when it interrupts a capture session.

class let interruptionEndedNotification: NSNotification.Name

A notification the system posts when an interruption to a capture session finishes.

class let runtimeErrorNotification: NSNotification.Name

A notification the system posts when an error occurs during a capture session.

