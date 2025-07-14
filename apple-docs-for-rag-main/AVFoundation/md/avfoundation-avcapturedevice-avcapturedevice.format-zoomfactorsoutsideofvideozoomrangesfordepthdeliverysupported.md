

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported 

Instance Property

# zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported

A Boolean value that indicates whether the format supports zoom factors outside the range supported for depth delivery.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+

``` source
var zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported: Bool { get }
```

## Discussion

Setting a zoom factor outside the range defined by the supportedVideoZoomFactorsForDepthDataDelivery property results in the system suspending depth data delivery. It resumes delivery when you set the zoom factor back to a supported value.

## See Also

### Determining Zoom Capabilities

var systemRecommendedVideoZoomRange: ClosedRange&lt;CGFloat>?

The system’s recommended zoom range for this device format.

var videoMaxZoomFactor: CGFloat

A maximum zoom factor the format allows.

var videoZoomFactorUpscaleThreshold: CGFloat

A threshold at which the system upscales pixel data.

var secondaryNativeResolutionZoomFactors: [CGFloat]

The zoom factors at which this device transitions to secondary native resolution modes.

var supportedVideoZoomRangesForDepthDataDelivery: [ClosedRange&lt;CGFloat>]

The zoom ranges that support the delivery of depth data.

