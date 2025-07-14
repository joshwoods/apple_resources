

- RoomPlan
- RoomCaptureSession
- RoomCaptureSession.CaptureError
-  RoomCaptureSession.CaptureError.internalError 

Case

# RoomCaptureSession.CaptureError.internalError

An error that indicates when the framework encounters an unexpected error case.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
case internalError
```

## See Also

### Identifying the error cause

case deviceNotSupported

An error that indicates that the framework doesn’t support the user’s device.

case deviceTooHot

An error that indicates when the device thermal metrics surpass the framework’s limitations.

case exceedSceneSizeLimit

An error that indicates when the scene size grows past the framework’s limitations.

case invalidARConfiguration

An error that indicates when the ARKit session runs an unsupported configuration.

case worldTrackingFailure

An error that indicates an issue with the underlying ARKit session.

