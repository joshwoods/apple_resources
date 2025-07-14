

- LockedCameraCapture
- LockedCameraCaptureUIScene
-  init(content:) 

Initializer

# init(content:)

Creates a locked camera capture extension scene.

iOS 18.0+iPadOS 18.0+

``` source
@MainActor
init(content: @escaping (LockedCameraCaptureSession) -> Content)
```

## Parameters 

`content`  

The content of the locked camera capture extension using a LockedCameraCaptureSession.

