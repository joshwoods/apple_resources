

- LockedCameraCapture
-  LockedCameraCaptureUIScene 

Structure

# LockedCameraCaptureUIScene

A structure that contains the session object and UI to display for the locked camera capture extension.

iOS 18.0+iPadOS 18.0+

``` source
@MainActor
struct LockedCameraCaptureUIScene where Content : View
```

## Topics

### Initializers

init(content: (LockedCameraCaptureSession) -> Content)

Creates a locked camera capture extension scene.

### Instance Properties

var body: some AppExtensionScene

The content and behavior of the locked camera capture extension’s UI.

let session: LockedCameraCaptureSession

An object that can request to open the extension’s containing app and receives session configuration updates.

### Type Aliases

typealias Body

The type for this scene’s body.

## Relationships

### Conforms To

- AppExtensionScene
- LockedCameraCaptureExtensionScene
- Sendable

## See Also

### Capture and launch

class LockedCameraCaptureSession

An object that can request to open the extension’s containing app and receives session configuration updates.

