

- AVFoundation
- AVCaptureDevice
-  setTorchModeOn(level:) 

Instance Method

# setTorchModeOn(level:)

Sets the illumination level when in torch mode.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func setTorchModeOn(level torchLevel: Float) throws
```

## Parameters 

`torchLevel`  

The new torch mode level. This value must be a floating-point number between `0.0` and `1.0`. To set the torch mode level to the currently available maximum, specify the constant maxAvailableTorchLevel for this parameter.

## Discussion

This method sets the torch mode to AVCaptureDevice.TorchMode.on and sets the level to the specified value. If the device doesn’t support this mode or if you specify a value for `torchLevel` that’s outside the accepted range, this method raises an exception. If the torch value is within the accepted range but greater than the currently supported maximum—perhaps because the device is overheating—this method returns false.

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, calling this method raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## See Also

### Configuring Torch Settings

var hasTorch: Bool

A Boolean value that specifies whether the capture device has a torch.

var isTorchAvailable: Bool

A Boolean value that indicates whether the torch is currently available for use.

var isTorchActive: Bool

A Boolean value that indicates whether the device’s torch is currently active.

var torchLevel: Float

The current torch brightness level.

var torchMode: AVCaptureDevice.TorchMode

The current torch mode.

enum TorchMode

Constants to specify the capture device’s torch mode.

func isTorchModeSupported(AVCaptureDevice.TorchMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified torch mode.

class let maxAvailableTorchLevel: Float

A constant that indicates to set the torch to its maximum level.

