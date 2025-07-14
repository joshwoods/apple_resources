

- RealityKit
- ObjectCaptureSession
-  ObjectCaptureSession.CaptureState 

Enumeration

# ObjectCaptureSession.CaptureState

State of the capture session.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
enum CaptureState
```

## Overview

A session starts in `.initializing` state and proceeds through the other states via use of function calls until it reaches an end state. A session is over when the capture state is set to `.completed` or `.failed(Error)`.

## Topics

### Operators

static func == (ObjectCaptureSession.CaptureState, ObjectCaptureSession.CaptureState) -> Bool

Two states are defined equal if they have the same case. Specifically, a `.failed(Error)` state will match any other failed state regardless of the actual error payload.

### Enumeration Cases

case capturing

Auto-capture is in progress.

case completed

The session has saved its data and can now be safely torn down and the images folder used for reconstruction.

case detecting

The object selection box is being detected / manipulated and is not yet complete. A call to `startCapturing()` in this state will move the session to `.capturing` to begin capturing the object indicated within the currently specified bounding box.

case failed(any Error)

There was an unrecoverable error and the session is now invalid and needs to be torn down.

case finishing

The session is saving outstanding data and finishing up.

case initializing

The session and camera feed are initializing.

case ready

The session is ready to begin taking calls to capture.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Monitoring the session

enum Error

Errors associated with the top-level computation of this class.

