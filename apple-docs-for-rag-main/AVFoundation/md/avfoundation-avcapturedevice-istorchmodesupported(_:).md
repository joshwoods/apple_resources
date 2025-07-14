

- AVFoundation
- AVCaptureDevice
-  isTorchModeSupported(\_:) 

Instance Method

# isTorchModeSupported(\_:)

Returns a Boolean value that indicates whether the device supports the specified torch mode.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func isTorchModeSupported(_ torchMode: AVCaptureDevice.TorchMode) -> Bool
```

## Parameters 

`torchMode`  

The desired torch mode.

## Return Value

true if the device supports the torch mode; otherwise, false.

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

func setTorchModeOn(level: Float) throws

Sets the illumination level when in torch mode.

class let maxAvailableTorchLevel: Float

A constant that indicates to set the torch to its maximum level.

