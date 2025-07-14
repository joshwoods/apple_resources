

- AVFoundation
- AVCaptureDevice
-  exposureTargetBias 

Instance Property

# exposureTargetBias

The bias to apply to the target exposure value, in exposure value (EV) units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var exposureTargetBias: Float { get }
```

## Mentioned in 

Enhancing your app experience with the Camera Control

## Discussion

When the device exposure mode is AVCaptureDevice.ExposureMode.continuousAutoExposure or AVCaptureDevice.ExposureMode.locked, the bias affects both metering (exposureTargetOffset), and the actual exposure level (exposureDuration and iso). When the exposure mode is AVCaptureDevice.ExposureMode.custom, it only affects metering.

This property is key-value observable.

## See Also

### Adjusting Exposure Compensation

var exposureTargetOffset: Float

The metered exposure level’s offset from the target exposure value, in exposure value (EV) units.

var minExposureTargetBias: Float

The minimum supported exposure bias, in exposure value (EV) units.

var maxExposureTargetBias: Float

The maximum supported exposure bias, in exposure value (EV) units.

class let currentExposureTargetBias: Float

A special constant that represents the current exposure bias value.

func setExposureTargetBias(Float, completionHandler: ((CMTime) -> Void)?)

Sets the bias to apply to the target exposure value.

