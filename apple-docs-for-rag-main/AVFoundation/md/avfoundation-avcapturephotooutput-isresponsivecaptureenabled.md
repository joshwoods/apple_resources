

- AVFoundation
- AVCapturePhotoOutput
-  isResponsiveCaptureEnabled 

Instance Property

# isResponsiveCaptureEnabled

A Boolean value that indicates whether the photo output configuration enables responsive capture.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var isResponsiveCaptureEnabled: Bool { get set }
```

## See Also

### Managing Responsive Capture

var captureReadiness: AVCapturePhotoOutput.CaptureReadiness

A value that specifies whether the photo output is ready to respond to new capture requests in a timely manner.

enum CaptureReadiness

Constants that indicate whether the output is ready to receive capture requests.

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

var isZeroShutterLagSupported: Bool

A Boolean value that indicates whether the photo output supports zero shutter lag.

var isZeroShutterLagEnabled: Bool

A Boolean value that indicates whether the photo output configuration enables zero shutter lag.

