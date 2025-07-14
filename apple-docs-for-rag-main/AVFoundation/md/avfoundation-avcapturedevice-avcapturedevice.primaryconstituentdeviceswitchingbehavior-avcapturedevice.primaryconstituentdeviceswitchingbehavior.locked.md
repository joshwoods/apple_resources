

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior
-  AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.locked 

Case

# AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior.locked

The device locks camera switching to the active primary constituent device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
case locked
```

## Discussion

A locked value restricts the minAvailableVideoZoomFactor property value to the switch-over zoom factor of the active primary constituent device. See virtualDeviceSwitchOverVideoZoomFactors for more information.

## See Also

### Switching Behaviors

case unsupported

The device doesn’t support constituent device switching.

case auto

The device automatically selects the best camera for the current scene.

case restricted

The device restricts fallback camera selection to certain conditions.

