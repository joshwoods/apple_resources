

- AVFoundation
- AVCaptureDevice
-  setWhiteBalanceModeLocked(with:completionHandler:) 

Instance Method

# setWhiteBalanceModeLocked(with:completionHandler:)

Sets the white balance to locked mode with the specified white balance gains.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func setWhiteBalanceModeLocked(
    with whiteBalanceGains: AVCaptureDevice.WhiteBalanceGains,
    completionHandler handler: ((CMTime) -> Void)? = nil
)
```

``` source
func setWhiteBalanceModeLocked(with whiteBalanceGains: AVCaptureDevice.WhiteBalanceGains) async -> CMTime
```

## Parameters 

`whiteBalanceGains`  

The white balance gains to set. Pass a value of currentWhiteBalanceGains to leave the current white balance unchanged.

`handler`  

A callback the system invokes when the adjustment to the white balance is complete and the whiteBalanceMode set to a locked state. If you call this method multiple times, the system calls the completion handlers in FIFO order.

The system passes a time value that matches that of the first buffer to which its applied all settings. It synchronizes the timestamp to the device clock, and you must convert the timestamp to the synchronizationClock prior to comparison with the timestamps of buffers delivered through an AVCaptureVideoDataOutput.

You can pass `nil` for this parameter if you don’t require this information.

## Discussion

Each channel in the white balance gains structure supports values between `1.0` and maxWhiteBalanceGain. Setting a channel value outside this range generates an exception.

The system normalizes gain values to the minimum channel value to avoid brightness changes (for example, `R:2 G:2 B:4` normalizes to `R:1 G:1 B:2`).

Before changing the value the white balance gains, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## Topics

### White Balance Constants

class let currentWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains

A special constant representing the current white balance setting.

## See Also

### Setting White Balance Manually

var isLockingWhiteBalanceWithCustomDeviceGainsSupported: Bool

A Boolean value that indicates whether the device supports locking white balance to specific gain values.

