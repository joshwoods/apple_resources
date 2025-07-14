

- AVFoundation
- AVCapturePhotoOutput
- AVCapturePhotoOutput.CaptureReadiness
-  AVCapturePhotoOutput.CaptureReadiness.notReadyWaitingForCapture 

Case

# AVCapturePhotoOutput.CaptureReadiness.notReadyWaitingForCapture

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy capturing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
case notReadyWaitingForCapture
```

## See Also

### Readiness states

case sessionNotRunning

Indicates that the session isn’t running and the output isn’t ready to receive requests.

case notReadyMomentarily

Indicates that the output isn’t ready to receive requests, but may be ready shortly.

case notReadyWaitingForProcessing

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy processing.

case ready

Indicates that the output is ready to receive new requests.

