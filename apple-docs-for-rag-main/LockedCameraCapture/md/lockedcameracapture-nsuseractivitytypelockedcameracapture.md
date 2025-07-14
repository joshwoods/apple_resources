

- LockedCameraCapture
-  NSUserActivityTypeLockedCameraCapture 

Global Variable

# NSUserActivityTypeLockedCameraCapture

A type to use when opening your app from the capture extension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
let NSUserActivityTypeLockedCameraCapture: String
```

## Discussion

Use this `NSUserActivityType` with openApplication(for:) to check if someone is launching your app from a locked camera capture extension.

## See Also

### App integration

class LockedCameraCaptureManager

An object that provides handling of captured content and transitioning to the extension’s containing app.

