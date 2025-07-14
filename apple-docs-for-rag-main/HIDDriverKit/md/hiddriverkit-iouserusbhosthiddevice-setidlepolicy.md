

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  setIdlePolicy 

Instance Method

# setIdlePolicy

Sets the amount of idle time that must pass before suspending the device.

DriverKit 19.0+macOS

``` source
kern_return_t setIdlePolicy(USBIdlePolicyType type, uint16_t idleTimeMs);
```

## Parameters 

`type`  

The target of the idle policy. For a list of possible values, see USBIdlePolicyType.

`idleTimeMs`  

The idle time in milliseconds.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Once the interface or pipe is idle, it defers electrical suspension of the device for the specified duration.

## See Also

### Configuring the Device

setProtocol

Sets the active protocol to use for communicating with the USB device.

setIdle

Sets the device’s idle time.

setProperty

Updates the specified property on the corresponding kernel object.

reset

Resets the USB device.

USBIdlePolicyType

Constants that specify whether to apply the idle policy to an interface or pipe.

