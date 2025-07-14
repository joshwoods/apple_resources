

- AVFoundation
- AVCaptureDevice
-  maxExposureTargetBias 

Instance Property

# maxExposureTargetBias

The maximum supported exposure bias, in exposure value (EV) units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var maxExposureTargetBias: Float { get }
```

## See Also

### Adjusting Exposure Compensation

var exposureTargetOffset: Float

The metered exposure level’s offset from the target exposure value, in exposure value (EV) units.

var exposureTargetBias: Float

The bias to apply to the target exposure value, in exposure value (EV) units.

var minExposureTargetBias: Float

The minimum supported exposure bias, in exposure value (EV) units.

class let currentExposureTargetBias: Float

A special constant that represents the current exposure bias value.

func setExposureTargetBias(Float, completionHandler: ((CMTime) -> Void)?)

Sets the bias to apply to the target exposure value.

