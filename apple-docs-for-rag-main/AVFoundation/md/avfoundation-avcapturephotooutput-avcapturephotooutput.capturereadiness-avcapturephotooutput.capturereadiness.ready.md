

- AVFoundation
- AVCapturePhotoOutput
- AVCapturePhotoOutput.CaptureReadiness
-  AVCapturePhotoOutput.CaptureReadiness.ready 

Case

# AVCapturePhotoOutput.CaptureReadiness.ready

Indicates that the output is ready to receive new requests.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
case ready
```

## See Also

### Readiness states

case sessionNotRunning

Indicates that the session isn’t running and the output isn’t ready to receive requests.

case notReadyMomentarily

Indicates that the output isn’t ready to receive requests, but may be ready shortly.

case notReadyWaitingForCapture

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy capturing.

case notReadyWaitingForProcessing

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy processing.

