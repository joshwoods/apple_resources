

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoMinZoomFactorForDepthDataDelivery Deprecated

Instance Property

# videoMinZoomFactorForDepthDataDelivery

A minimum zoom factor the device supports when configured for depth data delivery.

iOS 11.0–16.0DeprecatediPadOS 11.0–16.0DeprecatedMac Catalyst 14.0–16.0Deprecated

``` source
var videoMinZoomFactorForDepthDataDelivery: CGFloat { get }
```

Deprecated

Use supportedVideoZoomFactorsForDepthDataDelivery instead.

## Discussion

Depth data capture requires coordinating the zoom factors of the two cameras on a dual-camera device. Therefore, when you enable depth data delivery for a capture format using the AVCaptureDepthDataOutput class, the range of available values for the device’s videoZoomFactor property is reduced.

If this format doesn’t support depth capture, this property’s value is `1.0`.

## See Also

### Determining Zoom Capabilities

var supportedVideoZoomFactorsForDepthDataDelivery: [CGFloat]

The zoom factors that a format supports for depth data delivery.

Deprecated

var videoMaxZoomFactorForDepthDataDelivery: CGFloat

A maximum zoom factor the device supports when configured for depth data delivery.

Deprecated

