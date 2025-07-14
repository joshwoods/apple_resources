

- AVFoundation
- AVCaptureDevice
-  currentExposureTargetBias 

Type Property

# currentExposureTargetBias

A special constant that represents the current exposure bias value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class let currentExposureTargetBias: Float
```

## Discussion

Pass this value to the setExposureTargetBias(_:completionHandler:) method to lock exposure bias to its current value, which disables autoexposure.

## See Also

### Adjusting Exposure Compensation

var exposureTargetOffset: Float

The metered exposure level’s offset from the target exposure value, in exposure value (EV) units.

var exposureTargetBias: Float

The bias to apply to the target exposure value, in exposure value (EV) units.

var minExposureTargetBias: Float

The minimum supported exposure bias, in exposure value (EV) units.

var maxExposureTargetBias: Float

The maximum supported exposure bias, in exposure value (EV) units.

func setExposureTargetBias(Float, completionHandler: ((CMTime) -> Void)?)

Sets the bias to apply to the target exposure value.

