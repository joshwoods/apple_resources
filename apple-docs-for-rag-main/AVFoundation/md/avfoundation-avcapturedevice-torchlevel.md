

- AVFoundation
- AVCaptureDevice
-  torchLevel 

Instance Property

# torchLevel

The current torch brightness level.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var torchLevel: Float { get }
```

## Discussion

The value of this property is a floating-point number whose value is in the range 0.0 to 1.0. A torch level of 0.0 indicates that the torch is off. A torch level of 1.0 represents the theoretical maximum value, although the actual maximum value may be lower if the device is currently overheated.

This property is key-value observable.

## See Also

### Configuring Torch Settings

var hasTorch: Bool

A Boolean value that specifies whether the capture device has a torch.

var isTorchAvailable: Bool

A Boolean value that indicates whether the torch is currently available for use.

var isTorchActive: Bool

A Boolean value that indicates whether the device’s torch is currently active.

var torchMode: AVCaptureDevice.TorchMode

The current torch mode.

enum TorchMode

Constants to specify the capture device’s torch mode.

func isTorchModeSupported(AVCaptureDevice.TorchMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified torch mode.

func setTorchModeOn(level: Float) throws

Sets the illumination level when in torch mode.

class let maxAvailableTorchLevel: Float

A constant that indicates to set the torch to its maximum level.

