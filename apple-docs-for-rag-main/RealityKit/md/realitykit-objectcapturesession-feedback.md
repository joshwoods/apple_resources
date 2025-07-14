

- RealityKit
- ObjectCaptureSession
-  feedback 

Instance Property

# feedback

The current set of active `Feedback` states.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var feedback: Set { get }
```

## See Also

### Configuring a session

enum Feedback

Provides information about possible problems with the capture session.

var isPaused: Bool

A Boolean value that indicates if the capture session is paused.

var state: ObjectCaptureSession.CaptureState

The current state of the capture session.

var cameraTracking: ObjectCaptureSession.Tracking

The current state of ARKit camera tracking.

enum Tracking

A data structure that describes the current tracking state for the camera.

