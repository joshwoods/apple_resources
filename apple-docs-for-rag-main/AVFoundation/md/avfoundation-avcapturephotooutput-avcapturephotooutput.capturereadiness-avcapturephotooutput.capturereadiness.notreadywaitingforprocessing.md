

- AVFoundation
- AVCapturePhotoOutput
- AVCapturePhotoOutput.CaptureReadiness
-  AVCapturePhotoOutput.CaptureReadiness.notReadyWaitingForProcessing 

Case

# AVCapturePhotoOutput.CaptureReadiness.notReadyWaitingForProcessing

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy processing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
case notReadyWaitingForProcessing
```

## See Also

### Readiness states

case sessionNotRunning

Indicates that the session isn’t running and the output isn’t ready to receive requests.

case notReadyMomentarily

Indicates that the output isn’t ready to receive requests, but may be ready shortly.

case notReadyWaitingForCapture

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy capturing.

case ready

Indicates that the output is ready to receive new requests.

