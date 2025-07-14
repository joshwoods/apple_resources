

- HIDDriverKit
- IOHIDInterface
-  Open 

Instance Method

# Open

Opens a session to the device and begins the delivery of input reports.

DriverKit 19.0+macOS

``` source
kern_return_t Open(IOService * forClient, IOOptionBits options, OSAction * action);
```

## Parameters 

`forClient`  

The client that opened the interface.

`options`  

Options to use when opening the session. Specify `0` for no options.

`action`  

The `OSAction` object that handles the asynchronous report callback. The action’s callback must conform to the ReportAvailable method.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Managing the Session

Close

Closes the interface and stops the delivery of input reports.

