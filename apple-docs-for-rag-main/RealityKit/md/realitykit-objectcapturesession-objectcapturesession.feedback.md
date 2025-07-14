

- RealityKit
- ObjectCaptureSession
-  ObjectCaptureSession.Feedback 

Enumeration

# ObjectCaptureSession.Feedback

Provides information about possible problems with the capture session.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
enum Feedback
```

## Topics

### Operators

static func == (ObjectCaptureSession.Feedback, ObjectCaptureSession.Feedback) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case environmentLowLight

The lighting in the environment is low, which can degrade reconstruction quality. Auto-capture still proceeds but reconstruction quality may suffer. It is advised to increase lighting.

case environmentTooDark

The lighting in the environment is too dark to proceed. Auto-capture will stop and the user will need to increase lighting levels to resolve this condition in order to continue capture.

case movingTooFast

The user is moving too quickly for clear images and the capturing may be paused to ensure quality.

case objectNotDetected

If the detection of the object fails and a default manual box is presented instead, this element will be in the feedback to allow relevant information to be provided to the user for selecting a manual scanning volume and describing the operational envelope for the automatic object detection.

case objectNotFlippable

It is not recommended to flip this object since is is unlikely the algorithm will be able to stitch the flipped orientation. This is usually due to feature-less, low-texture objects. In this case, multiple passes at different heights leaving object at its original orientation are recommended instead of flipping.

case objectTooClose

The camera is too close to the object and it cannot be tracked well.

case objectTooFar

The camera is too far from the object and it cannot be captured well.

case outOfFieldOfView

The bounding box of the object is not in the field of view of the camera so auto-capture will not operate.

case overCapturing

If the `numberOfShotsTaken > maximumNumberOfInputImages` then any additional shots will not be used in an on-device reconstruction and reconstruction is recommended to be done on a Mac that can support a greater number of images.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Configuring a session

var feedback: Set&lt;ObjectCaptureSession.Feedback>

The current set of active `Feedback` states.

var isPaused: Bool

A Boolean value that indicates if the capture session is paused.

var state: ObjectCaptureSession.CaptureState

The current state of the capture session.

var cameraTracking: ObjectCaptureSession.Tracking

The current state of ARKit camera tracking.

enum Tracking

A data structure that describes the current tracking state for the camera.

