

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  setProtocol 

Instance Method

# setProtocol

Sets the active protocol to use for communicating with the USB device.

DriverKit 19.0+macOS

``` source
kern_return_t setProtocol(uint16_t protocol);
```

## Parameters 

`protocol`  

The protocol to use for the device. Specify `0` to use the boot protocol or `1` to use the report protocol.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

At startup, the Start method sets the protocol to the report protocol.

## See Also

### Configuring the Device

setIdle

Sets the device’s idle time.

setIdlePolicy

Sets the amount of idle time that must pass before suspending the device.

setProperty

Updates the specified property on the corresponding kernel object.

reset

Resets the USB device.

USBIdlePolicyType

Constants that specify whether to apply the idle policy to an interface or pipe.

