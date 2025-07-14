

- USBDriverKit
- IOUSBHostInterface
-  Open 

Instance Method

# Open

Opens a session to the host interface.

DriverKit 19.0+

``` source
kern_return_t Open(IOService * forClient, IOOptionBits options, uint8_t * arg);
```

## Parameters 

`forClient`  

The service object that is opening the session.

`options`  

The options to use when opening the session. Specify kUSBHostOpenOptionSelectAlternateSetting to select an alternative setting for this interface immediately. Specify the alternative setting in the `arg` parameter.

`arg`  

Additional arguments to the function. If you specify kUSBHostOpenOptionSelectAlternateSetting for the `options` parameter, use this value to specify the value for the alternative setting; otherwise, specify `NULL`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method opens a session to the IOUSBHostInterface, and acquires the service’s workloop lock. Only one service at a time may open a session to the interface.

## See Also

### Managing the Device Session

Close

Closes the session to the host interface.

