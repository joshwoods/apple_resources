

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoFrameRateRangeForPortraitEffect 

Instance Property

# videoFrameRateRangeForPortraitEffect

The range of frame rates available when Portrait Effect is active.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var videoFrameRateRangeForPortraitEffect: AVFrameRateRange? { get }
```

## Discussion

Devices may support a limited range of frame rates when Portrait Effect is active. If a device format doesn’t support Portrait Effect, the value of this property is `nil`.

## See Also

### Determining Portrait Effects Support

var isPortraitEffectSupported: Bool

A Boolean value that indicates whether the format supports the Portrait Effect feature.

var isPortraitEffectsMatteStillImageDeliverySupported: Bool

A Boolean indicating whether the device supports portrait matte effects in still-image capture.

