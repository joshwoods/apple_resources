

- AVFoundation
- AVCaptureDevice
-  currentWhiteBalanceGains 

Type Property

# currentWhiteBalanceGains

A special constant representing the current white balance setting.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class let currentWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains
```

## Discussion

Pass this value to setWhiteBalanceModeLocked(with:completionHandler:) to lock white balance gains to their current value (that is, disable automatic white balancing).

