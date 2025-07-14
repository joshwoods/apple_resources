

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  secondaryNativeResolutionZoomFactors 

Instance Property

# secondaryNativeResolutionZoomFactors

The zoom factors at which this device transitions to secondary native resolution modes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
@nonobjc
var secondaryNativeResolutionZoomFactors: [CGFloat] { get }
```

## Discussion

Devices that provide secondary native resolution zoom factors can switch their pixel sampling mode dynamically to produce high-fidelity images without upscaling at a fixed zoom factor beyond `1.0`.

## See Also

### Determining Zoom Capabilities

var systemRecommendedVideoZoomRange: ClosedRange&lt;CGFloat>?

The system’s recommended zoom range for this device format.

var videoMaxZoomFactor: CGFloat

A maximum zoom factor the format allows.

var videoZoomFactorUpscaleThreshold: CGFloat

A threshold at which the system upscales pixel data.

var supportedVideoZoomRangesForDepthDataDelivery: [ClosedRange&lt;CGFloat>]

The zoom ranges that support the delivery of depth data.

var zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported: Bool

A Boolean value that indicates whether the format supports zoom factors outside the range supported for depth delivery.

