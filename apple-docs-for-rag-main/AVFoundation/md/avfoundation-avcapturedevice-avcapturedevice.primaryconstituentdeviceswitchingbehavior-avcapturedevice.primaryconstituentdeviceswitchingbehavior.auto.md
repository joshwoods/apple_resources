

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior
-  AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.auto 

Case

# AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.auto

The device automatically selects the best camera for the current scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
case auto
```

## Discussion

This mode places no restrictions on when a camera switch can occur.

## See Also

### Switching Behaviors

case unsupported

The device doesn’t support constituent device switching.

case restricted

The device restricts fallback camera selection to certain conditions.

case locked

The device locks camera switching to the active primary constituent device.

