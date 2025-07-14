

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoZoomFactorUpscaleThreshold 

Instance Property

# videoZoomFactorUpscaleThreshold

A threshold at which the system upscales pixel data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var videoZoomFactorUpscaleThreshold: CGFloat { get }
```

## Discussion

The device achieves a zoom effect by cropping around the center of the image captured by the sensor. At low zoom factors, the cropped images is equal to or larger than the output size. At higher zoom factors, the device must scale the cropped image up to the output size, resulting in a loss of image quality. This property indicates the factors at which upscaling occurs.

## See Also

### Determining Zoom Capabilities

var systemRecommendedVideoZoomRange: ClosedRange&lt;CGFloat>?

The system’s recommended zoom range for this device format.

var videoMaxZoomFactor: CGFloat

A maximum zoom factor the format allows.

var secondaryNativeResolutionZoomFactors: [CGFloat]

The zoom factors at which this device transitions to secondary native resolution modes.

var supportedVideoZoomRangesForDepthDataDelivery: [ClosedRange&lt;CGFloat>]

The zoom ranges that support the delivery of depth data.

var zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported: Bool

A Boolean value that indicates whether the format supports zoom factors outside the range supported for depth delivery.

