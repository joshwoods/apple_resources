

- AVFoundation
- AVCaptureDevice
-  hasTorch 

Instance Property

# hasTorch

A Boolean value that specifies whether the capture device has a torch.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var hasTorch: Bool { get }
```

## Discussion

A torch is a light source, such as an LED flash, that’s available on the device and used for illuminating captured content or providing general illumination. This property reflects whether the current device has such illumination hardware built-in.

Even if the device has a torch, that torch might not be available for use, so check the value of the isTorchAvailable property before using it.

This property is key-value observable.

## See Also

### Configuring Torch Settings

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

func setTorchModeOn(level: Float) throws

Sets the illumination level when in torch mode.

class let maxAvailableTorchLevel: Float

A constant that indicates to set the torch to its maximum level.

