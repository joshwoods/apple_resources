

- RealityKit
- ObjectCaptureSession
-  isPaused 

Instance Property

# isPaused

A Boolean value that indicates if the capture session is paused.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var isPaused: Bool { get }
```

## See Also

### Configuring a session

var feedback: Set&lt;ObjectCaptureSession.Feedback>

The current set of active `Feedback` states.

enum Feedback

Provides information about possible problems with the capture session.

var state: ObjectCaptureSession.CaptureState

The current state of the capture session.

var cameraTracking: ObjectCaptureSession.Tracking

The current state of ARKit camera tracking.

enum Tracking

A data structure that describes the current tracking state for the camera.

