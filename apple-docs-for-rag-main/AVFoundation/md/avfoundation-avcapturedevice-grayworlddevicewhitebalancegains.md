

- AVFoundation
- AVCaptureDevice
-  grayWorldDeviceWhiteBalanceGains 

Instance Property

# grayWorldDeviceWhiteBalanceGains

The current device-specific white balance values required for a neutral gray white point.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var grayWorldDeviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains { get }
```

## Discussion

This property specifies the current red, green, and blue gain values derived from the current scene to deliver a neutral (or gray world) white point for white balance.

Gray world values assume you’ve placed a neutral subject (for example, a gray card) in the middle of the subject area, and fills the center 50% of the frame. Apps can read these values and apply them to the device using setWhiteBalanceModeLocked(with:completionHandler:).

Each change supports values between `1.0` and maxWhiteBalanceGain. You can read the value at any time, regardless of white balance mode.

This property is key-value observable.

## See Also

### Inspecting Gain Levels

var deviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains

The current device-specific RGB white balance gain values in use.

var maxWhiteBalanceGain: Float

The maximum supported value to which you can set a color channel.

