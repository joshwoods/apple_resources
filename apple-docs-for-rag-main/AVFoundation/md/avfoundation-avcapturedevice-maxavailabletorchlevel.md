

- AVFoundation
- AVCaptureDevice
-  maxAvailableTorchLevel 

Type Property

# maxAvailableTorchLevel

A constant that indicates to set the torch to its maximum level.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
class let maxAvailableTorchLevel: Float
```

## Discussion

Pass this value to the setTorchModeOn(level:) method to set the torch to the maximum level currently available. Under thermal duress, the maximum available torch level may be less than 1.0.

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

func setTorchModeOn(level: Float) throws

Sets the illumination level when in torch mode.

