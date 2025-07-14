

- LockedCameraCapture
- LockedCameraCaptureUIScene
-  session 

Instance Property

# session

An object that can request to open the extension’s containing app and receives session configuration updates.

iOS 18.0+iPadOS 18.0+

``` source
@MainActor
let session: LockedCameraCaptureSession
```

## Discussion

Provided during the initialization of the LockedCameraCaptureExtensionScene. Only the system can initialize this object.

