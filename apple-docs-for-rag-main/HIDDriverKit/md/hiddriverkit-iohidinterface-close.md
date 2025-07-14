

- HIDDriverKit
- IOHIDInterface
-  Close 

Instance Method

# Close

Closes the interface and stops the delivery of input reports.

DriverKit 19.0+macOS

``` source
kern_return_t Close(IOService * forClient, IOOptionBits options);
```

## Parameters 

`forClient`  

The client that closed the interface.

`options`  

Options to use when closing the session. Specify `0` for no options.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Managing the Session

Open

Opens a session to the device and begins the delivery of input reports.

