

- HIDDriverKit
-  USBIdlePolicyType 

Enumeration

# USBIdlePolicyType

Constants that specify whether to apply the idle policy to an interface or pipe.

DriverKitmacOS

``` source
typedef enum { ... } USBIdlePolicyType;
```

## Topics

### Getting the Idle Policy

USBIdlePolicyTypeInterface

An idle policy that applies to the interface connected to the device.

USBIdlePolicyTypePipe

An idle policy that applies to the pipe that communicates with the device.

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

reset

Resets the USB device.

