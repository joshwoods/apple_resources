

- AVFoundation
- AVCaptureDevice
-  maxWhiteBalanceGain 

Instance Property

# maxWhiteBalanceGain

The maximum supported value to which you can set a color channel.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var maxWhiteBalanceGain: Float { get }
```

## Discussion

This property doesn’t change for the life of the object.

## See Also

### Inspecting Gain Levels

var deviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains

The current device-specific RGB white balance gain values in use.

var grayWorldDeviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains

The current device-specific white balance values required for a neutral gray white point.

