

- AVFoundation
- AVCaptureDevice
-  deviceWhiteBalanceGains 

Instance Property

# deviceWhiteBalanceGains

The current device-specific RGB white balance gain values in use.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var deviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains { get }
```

## Discussion

This property specifies the current red, green, and blue gain values used for white balance. You can use the values to adjust color casts for a given scene. Each channel supports values between 1.0 and -maxWhiteBalanceGain.

This property is key-value observable.

## See Also

### Inspecting Gain Levels

var grayWorldDeviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains

The current device-specific white balance values required for a neutral gray white point.

var maxWhiteBalanceGain: Float

The maximum supported value to which you can set a color channel.

