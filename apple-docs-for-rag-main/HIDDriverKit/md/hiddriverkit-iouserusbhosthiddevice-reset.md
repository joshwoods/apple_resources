

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  reset 

Instance Method

# reset

Resets the USB device.

DriverKit 19.0+macOS

``` source
void reset();
```

## See Also

### Configuring the Device

setProtocol

Sets the active protocol to use for communicating with the USB device.

setIdle

Sets the device’s idle time.

setIdlePolicy

Sets the amount of idle time that must pass before suspending the device.

setProperty

Updates the specified property on the corresponding kernel object.

USBIdlePolicyType

Constants that specify whether to apply the idle policy to an interface or pipe.

