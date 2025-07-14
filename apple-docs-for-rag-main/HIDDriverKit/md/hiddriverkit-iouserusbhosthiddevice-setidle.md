

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  setIdle 

Instance Method

# setIdle

Sets the device’s idle time.

DriverKit 19.0+macOS

``` source
kern_return_t setIdle(uint16_t idleTimeMs);
```

## Parameters 

`idleTimeMs`  

The idle time in milliseconds.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

The idle rate determines how often a device resends data that hasn’t changed since the last report. Use this method to limit the reporting frequency of an interrupt `IN` endpoint.

## See Also

### Configuring the Device

setProtocol

Sets the active protocol to use for communicating with the USB device.

setIdlePolicy

Sets the amount of idle time that must pass before suspending the device.

setProperty

Updates the specified property on the corresponding kernel object.

reset

Resets the USB device.

USBIdlePolicyType

Constants that specify whether to apply the idle policy to an interface or pipe.

