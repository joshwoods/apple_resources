

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior
-  AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.restricted 

Case

# AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.restricted

The device restricts fallback camera selection to certain conditions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
case restricted
```

## Discussion

The camera doesn’t restrict camera switches necessary to honor the requested video zoom factor.

## See Also

### Switching Behaviors

case unsupported

The device doesn’t support constituent device switching.

case auto

The device automatically selects the best camera for the current scene.

case locked

The device locks camera switching to the active primary constituent device.

