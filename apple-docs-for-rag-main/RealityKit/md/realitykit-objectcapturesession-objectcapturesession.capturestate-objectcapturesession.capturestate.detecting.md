

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.CaptureState
-  ObjectCaptureSession.CaptureState.detecting 

Case

# ObjectCaptureSession.CaptureState.detecting

The object selection box is being detected / manipulated and is not yet complete. A call to `startCapturing()` in this state will move the session to `.capturing` to begin capturing the object indicated within the currently specified bounding box.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
case detecting
```

