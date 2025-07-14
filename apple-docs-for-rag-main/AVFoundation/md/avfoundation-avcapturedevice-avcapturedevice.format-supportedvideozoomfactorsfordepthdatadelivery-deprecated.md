

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  supportedVideoZoomFactorsForDepthDataDelivery Deprecated

Instance Property

# supportedVideoZoomFactorsForDepthDataDelivery

The zoom factors that a format supports for depth data delivery.

iOS 16.0–17.2DeprecatediPadOS 16.0–17.2DeprecatedMac Catalyst 16.0–17.2DeprecatedtvOS 17.0–17.2Deprecated

``` source
@nonobjc
var supportedVideoZoomFactorsForDepthDataDelivery: [CGFloat] { get }
```

Deprecated

Use AVCaptureDevice.Format.supportedVideoZoomRangesForDepthDataDelivery instead

## See Also

### Determining Zoom Capabilities

var videoMinZoomFactorForDepthDataDelivery: CGFloat

A minimum zoom factor the device supports when configured for depth data delivery.

Deprecated

var videoMaxZoomFactorForDepthDataDelivery: CGFloat

A maximum zoom factor the device supports when configured for depth data delivery.

Deprecated

