

- LockedCameraCapture
- LockedCameraCaptureSession
-  openApplication(for:) 

Instance Method

# openApplication(for:)

Initiates a request to open the extension’s containing app.

iOS 18.0+iPadOS 18.0+

``` source
final func openApplication(for userActivity: NSUserActivity) async throws
```

## Parameters 

`userActivity`  

An `NSUserActivity` that contains relevant information to benefit from universal link support. Use the NSUserActivityTypeLockedCameraCapture activity type to indicate when the app launches from a locked camera capture extension.

## Discussion

The system requests authentication before opening the app, if needed.

