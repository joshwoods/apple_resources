

- USBDriverKit
- IOUSBHostDevice
-  Open 

Instance Method

# Open

Opens a session to a host device.

DriverKit 19.0+

``` source
kern_return_t Open(IOService * forClient, IOOptionBits options, uintptr_t arg);
```

## Parameters 

`forClient`  

The service object that is opening the session.

`options`  

The options to use when opening the session. Specify `0` for this parameter.

`arg`  

Additional arguments to the function. Specify `NULL` for this parameter.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method opens a session to the IOUSBHostDevice, and acquires the service’s workloop lock. Child IOUSBHostInterface objects may open simultaneous sessions, but only one IOUSBHostDevice object at a time may open a session to the device.

## See Also

### Managing the Device Session

Close

Closes the session to the host device.

Reset

Terminates the device and attempts to reenumerate it.

