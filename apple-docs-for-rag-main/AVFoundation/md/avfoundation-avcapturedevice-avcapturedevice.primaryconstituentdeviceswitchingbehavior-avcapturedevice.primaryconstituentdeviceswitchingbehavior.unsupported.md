

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior
-  AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.unsupported 

Case

# AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.unsupported

The device doesn’t support constituent device switching.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
case unsupported
```

## Discussion

Switching cameras isn’t supported on devices that don’t have more than one constituent device.

## See Also

### Switching Behaviors

case auto

The device automatically selects the best camera for the current scene.

case restricted

The device restricts fallback camera selection to certain conditions.

case locked

The device locks camera switching to the active primary constituent device.

