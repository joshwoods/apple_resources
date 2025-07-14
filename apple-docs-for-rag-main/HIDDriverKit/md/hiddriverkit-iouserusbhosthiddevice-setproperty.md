

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  setProperty 

Instance Method

# setProperty

Updates the specified property on the corresponding kernel object.

DriverKit 19.0+macOS

``` source
void setProperty(OSObject * key, OSObject * value);
```

## Parameters 

`key`  

The property key.

`value`  

The property value.

## See Also

### Configuring the Device

setProtocol

Sets the active protocol to use for communicating with the USB device.

setIdle

Sets the device’s idle time.

setIdlePolicy

Sets the amount of idle time that must pass before suspending the device.

reset

Resets the USB device.

USBIdlePolicyType

Constants that specify whether to apply the idle policy to an interface or pipe.

