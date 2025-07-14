

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isPortraitEffectSupported 

Instance Property

# isPortraitEffectSupported

A Boolean value that indicates whether the format supports the Portrait Effect feature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var isPortraitEffectSupported: Bool { get }
```

## Discussion

Enabling a Portrait Effect applies a shallow depth-of-field effect to objects in the background. See the isPortraitEffectEnabled property of AVCaptureDevice for more information.

## See Also

### Determining Portrait Effects Support

var isPortraitEffectsMatteStillImageDeliverySupported: Bool

A Boolean indicating whether the device supports portrait matte effects in still-image capture.

var videoFrameRateRangeForPortraitEffect: AVFrameRateRange?

The range of frame rates available when Portrait Effect is active.

