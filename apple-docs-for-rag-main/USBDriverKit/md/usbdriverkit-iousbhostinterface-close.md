

- USBDriverKit
- IOUSBHostInterface
-  Close 

Instance Method

# Close

Closes the session to the host interface.

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

This method closes a session to an interface that you previously opened using the Open method. The method acquires the service’s workloop lock, and aborts any I/O for the interface and its endpoints. This method may also call commandSleep to allow for the processing of aborted I/O before returning.

## See Also

### Managing the Device Session

Open

Opens a session to the host interface.

