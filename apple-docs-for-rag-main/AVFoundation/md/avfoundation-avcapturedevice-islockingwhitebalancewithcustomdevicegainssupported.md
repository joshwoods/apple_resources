

- AVFoundation
- AVCaptureDevice
-  isLockingWhiteBalanceWithCustomDeviceGainsSupported 

Instance Property

# isLockingWhiteBalanceWithCustomDeviceGainsSupported

A Boolean value that indicates whether the device supports locking white balance to specific gain values.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLockingWhiteBalanceWithCustomDeviceGainsSupported: Bool { get }
```

## Discussion

If the value is false, calling the setWhiteBalanceModeLocked(with:completionHandler:) method with a white balance gains value other than currentWhiteBalanceGains throws an exception.

## See Also

### Setting White Balance Manually

func setWhiteBalanceModeLocked(with: AVCaptureDevice.WhiteBalanceGains, completionHandler: ((CMTime) -> Void)?)

Sets the white balance to locked mode with the specified white balance gains.

