

- RealityKit
- ObjectCaptureSession
-  cameraTracking 

Instance Property

# cameraTracking

The current state of ARKit camera tracking.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var cameraTracking: ObjectCaptureSession.Tracking { get }
```

## Discussion

The ARKit coaching overylay will be automatically show if this state moves away from `.normal` since the loss of ARKit tracking will cause many of the Object Capture algorithms to pause until the environmental tracking issue is resolved by the user. Also, the app may want to adjust its UI when this state is not `.normal` to allow proper visibility of the coaching overlay.

## See Also

### Configuring a session

var feedback: Set&lt;ObjectCaptureSession.Feedback>

The current set of active `Feedback` states.

enum Feedback

Provides information about possible problems with the capture session.

var isPaused: Bool

A Boolean value that indicates if the capture session is paused.

var state: ObjectCaptureSession.CaptureState

The current state of the capture session.

enum Tracking

A data structure that describes the current tracking state for the camera.

