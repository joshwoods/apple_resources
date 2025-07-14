

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  systemRecommendedVideoZoomRange 

Instance Property

# systemRecommendedVideoZoomRange

The system’s recommended zoom range for this device format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
@nonobjc
var systemRecommendedVideoZoomRange: ClosedRange? { get }
```

## Discussion

Use this value to create a slider in your app’s user interface that controls a device’s zoom within a system-recommended range. When a recommendation isn’t available, this property returns `nil`.

Apps can key-value observe a capture device’s minAvailableVideoZoomFactor and maxAvailableVideoZoomFactor property values to know when a device limits its supported zoom to the recommended range.

Note

The framework uses this value to define the range of an AVCaptureSystemZoomSlider control.

## See Also

### Determining Zoom Capabilities

var videoMaxZoomFactor: CGFloat

A maximum zoom factor the format allows.

var videoZoomFactorUpscaleThreshold: CGFloat

A threshold at which the system upscales pixel data.

var secondaryNativeResolutionZoomFactors: [CGFloat]

The zoom factors at which this device transitions to secondary native resolution modes.

var supportedVideoZoomRangesForDepthDataDelivery: [ClosedRange&lt;CGFloat>]

The zoom ranges that support the delivery of depth data.

var zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported: Bool

A Boolean value that indicates whether the format supports zoom factors outside the range supported for depth delivery.

