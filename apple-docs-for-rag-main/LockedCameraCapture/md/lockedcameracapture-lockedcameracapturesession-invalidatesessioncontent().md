

- LockedCameraCapture
- LockedCameraCaptureSession
-  invalidateSessionContent() 

Instance Method

# invalidateSessionContent()

Invalidates the contents of the session contents URL, deleting them. Note this does not remove the contents directory itself. This is useful in case the extension has already ingested its contents via PhotoKit and wishes to not persist any data (but can still use this directory as a working directory to recover from an unexpected termination).

iOS 18.0+iPadOS 18.0+

``` source
final func invalidateSessionContent() async throws
```

