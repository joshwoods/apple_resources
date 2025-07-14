

- AVFoundation
- AVCaptureDevice
-  exposureTargetOffset 

Instance Property

# exposureTargetOffset

The metered exposure level’s offset from the target exposure value, in exposure value (EV) units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var exposureTargetOffset: Float { get }
```

## Discussion

The value of property indicates the difference between the metered exposure level of the current scene and the target exposure value.

This property is key-value observable.

## See Also

### Adjusting Exposure Compensation

var exposureTargetBias: Float

The bias to apply to the target exposure value, in exposure value (EV) units.

var minExposureTargetBias: Float

The minimum supported exposure bias, in exposure value (EV) units.

var maxExposureTargetBias: Float

The maximum supported exposure bias, in exposure value (EV) units.

class let currentExposureTargetBias: Float

A special constant that represents the current exposure bias value.

func setExposureTargetBias(Float, completionHandler: ((CMTime) -> Void)?)

Sets the bias to apply to the target exposure value.

