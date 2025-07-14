

- AVFoundation
- AVCapturePhotoOutput
-  isAutoDeferredPhotoDeliveryEnabled 

Instance Property

# isAutoDeferredPhotoDeliveryEnabled

A Boolean value that indicates the enabled state of automatic deferred photo delivery.

iOS 17.0+iPadOS 17.0+

``` source
var isAutoDeferredPhotoDeliveryEnabled: Bool { get set }
```

## Discussion

Changing this value requires a lengthy reconfiguration of the capture pipeline, so you should set this property before calling startRunning() on the capture session.

Setting this property to true throws an invalid argument exception the value of isAutoDeferredPhotoDeliverySupported is false.

## See Also

### Managing Responsive Capture

var captureReadiness: AVCapturePhotoOutput.CaptureReadiness

A value that specifies whether the photo output is ready to respond to new capture requests in a timely manner.

enum CaptureReadiness

Constants that indicate whether the output is ready to receive capture requests.

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

