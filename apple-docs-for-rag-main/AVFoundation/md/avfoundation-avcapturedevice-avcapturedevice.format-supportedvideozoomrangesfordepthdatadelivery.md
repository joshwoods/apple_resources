

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  supportedVideoZoomRangesForDepthDataDelivery 

Instance Property

# supportedVideoZoomRangesForDepthDataDelivery

The zoom ranges that support the delivery of depth data.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+

``` source
@nonobjc
var supportedVideoZoomRangesForDepthDataDelivery: [ClosedRange] { get }
```

## Discussion

Virtual devices support limited zoom ranges when delivering depth data to any output. If a device format has no supportedDepthDataFormats, the value of this property is an empty array.

The presence of one or more ranges where the minimum and maximum zoom factors aren’t equal means the system supports continuous zoom with depth. For example, if the value of this property contains the closed ranges `2...2` and `4...4`, the system only allows you to set zoom factors 2 and 4 when you enable depth data delivery. Setting a zoom factor outside these ranges results in an exception. Alternatively, a closed range of `2...5` indicates the system supports depth data delivery with zoom factors from 2 to 5. You can set a zoom factor outside this range, but results in a loss of depth data. Setting the zoom factor back to the supported range resumes depth data delivery.

When you enable depth data delivery, the effective videoZoomFactorUpscaleThreshold is `1.0`, which means that all zoom factors that aren’t native zoom factors (see virtualDeviceSwitchOverVideoZoomFactors and secondaryNativeResolutionZoomFactors) result in digital upscaling.

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

var zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported: Bool

A Boolean value that indicates whether the format supports zoom factors outside the range supported for depth delivery.

