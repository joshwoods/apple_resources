

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoMaxZoomFactor 

Instance Property

# videoMaxZoomFactor

A maximum zoom factor the format allows.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var videoMaxZoomFactor: CGFloat { get }
```

## Discussion

A maximum factor of `1.0` indicates that the format isn’t capable of zooming.

## See Also

### Determining Zoom Capabilities

var systemRecommendedVideoZoomRange: ClosedRange&lt;CGFloat>?

The system’s recommended zoom range for this device format.

var videoZoomFactorUpscaleThreshold: CGFloat

A threshold at which the system upscales pixel data.

var secondaryNativeResolutionZoomFactors: [CGFloat]

The zoom factors at which this device transitions to secondary native resolution modes.

var supportedVideoZoomRangesForDepthDataDelivery: [ClosedRange&lt;CGFloat>]

The zoom ranges that support the delivery of depth data.

var zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported: Bool

A Boolean value that indicates whether the format supports zoom factors outside the range supported for depth delivery.

