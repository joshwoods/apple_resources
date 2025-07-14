

- AVFoundation
- AVCapturePhotoOutput
-  AVCapturePhotoOutput.CaptureReadiness 

Enumeration

# AVCapturePhotoOutput.CaptureReadiness

Constants that indicate whether the output is ready to receive capture requests.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
enum CaptureReadiness
```

## Topics

### Readiness states

case sessionNotRunning

Indicates that the session isn’t running and the output isn’t ready to receive requests.

case notReadyMomentarily

Indicates that the output isn’t ready to receive requests, but may be ready shortly.

case notReadyWaitingForCapture

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy capturing.

case notReadyWaitingForProcessing

Indicates that the output isn’t ready to receive requests for a longer duration because it’s busy processing.

case ready

Indicates that the output is ready to receive new requests.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Responsive Capture

var captureReadiness: AVCapturePhotoOutput.CaptureReadiness

A value that specifies whether the photo output is ready to respond to new capture requests in a timely manner.

var isAutoDeferredPhotoDeliveryEnabled: Bool

A Boolean value that indicates the enabled state of automatic deferred photo delivery.

var isAutoDeferredPhotoDeliverySupported: Bool

A Boolean value that indicates whether the photo output supports deferred photo delivery.

var isFastCapturePrioritizationSupported: Bool

A Boolean value that indicates whether the photo output supports fast capture prioritization.

var isFastCapturePrioritizationEnabled: Bool

A Boolean value that indicates whether the output enables fast capture prioritization.

var isResponsiveCaptureSupported: Bool

A Boolean value that indicates whether the photo output supports responsive capture.

var isResponsiveCaptureEnabled: Bool

A Boolean value that indicates whether the photo output configuration enables responsive capture.

var isZeroShutterLagSupported: Bool

A Boolean value that indicates whether the photo output supports zero shutter lag.

var isZeroShutterLagEnabled: Bool

A Boolean value that indicates whether the photo output configuration enables zero shutter lag.

