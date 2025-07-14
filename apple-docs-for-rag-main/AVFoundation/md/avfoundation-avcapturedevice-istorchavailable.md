

- AVFoundation
- AVCaptureDevice
-  isTorchAvailable 

Instance Property

# isTorchAvailable

A Boolean value that indicates whether the torch is currently available for use.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var isTorchAvailable: Bool { get }
```

## Discussion

The torch may become unavailable if, for example, the device overheats and needs to cool off.

This property is key-value observable.

## See Also

### Configuring Torch Settings

var hasTorch: Bool

A Boolean value that specifies whether the capture device has a torch.

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

