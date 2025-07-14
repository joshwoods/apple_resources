

- USBDriverKit
- IOUSBHostDevice
-  Close 

Instance Method

# Close

Closes the session to the host device.

DriverKit 19.0+

``` source
kern_return_t Close(IOService * forClient, IOOptionBits options);
```

## Parameters 

`forClient`  

The service object that is closing the session.

`options`  

Options to use when closing the service. Specify `0` for this parameter.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method closes a session to a device that you previously opened using the Open method. The method acquires the service’s workloop lock, and aborts any I/O initiated by the client service. This method may call commandSleep to allow for the processing of aborted I/O before returning.

## See Also

### Managing the Device Session

Open

Opens a session to a host device.

Reset

Terminates the device and attempts to reenumerate it.

