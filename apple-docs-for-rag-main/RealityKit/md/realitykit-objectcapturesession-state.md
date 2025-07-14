

- RealityKit
- ObjectCaptureSession
-  state 

Instance Property

# state

The current state of the capture session.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var state: ObjectCaptureSession.CaptureState { get }
```

## See Also

### Configuring a session

var feedback: Set&lt;ObjectCaptureSession.Feedback>

The current set of active `Feedback` states.

enum Feedback

Provides information about possible problems with the capture session.

var isPaused: Bool

A Boolean value that indicates if the capture session is paused.

var cameraTracking: ObjectCaptureSession.Tracking

The current state of ARKit camera tracking.

enum Tracking

A data structure that describes the current tracking state for the camera.

