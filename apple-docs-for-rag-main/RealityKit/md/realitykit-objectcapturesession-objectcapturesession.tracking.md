

- RealityKit
- ObjectCaptureSession
-  ObjectCaptureSession.Tracking 

Enumeration

# ObjectCaptureSession.Tracking

A data structure that describes the current tracking state for the camera.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
enum Tracking
```

## Overview

During an object capture, many factors contribute to the session’s ability to accurately track the position and orientation of the camera and object, including lighting and enough texture on the object and background. The object capture session uses this data structure to report the current tracking state in the cameraTracking property. Additionally, the ARKit coaching overlay will automatically appear when tracking is not `.normal` — the app may need to hide its UI at this time as well to allow proper visibility of the coaching overlay or to provide additional information to the user to correct the situation.

## Topics

### Operators

static func == (ObjectCaptureSession.Tracking, ObjectCaptureSession.Tracking) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case limited(reason: ObjectCaptureSession.Tracking.Reason)

Tracking is available but its quality is degraded. The ARKit coaching overlay will appear when cameraTracking enters this state.

case normal

Tracking is available and the session detects no problems..

case notAvailable

Tracking is not yet available.

### Enumerations

enum Reason

The reason that tracking quality has degraded.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

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

var cameraTracking: ObjectCaptureSession.Tracking

The current state of ARKit camera tracking.

