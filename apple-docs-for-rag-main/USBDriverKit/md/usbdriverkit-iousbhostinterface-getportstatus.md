

- USBDriverKit
- IOUSBHostInterface
-  GetPortStatus 

Instance Method

# GetPortStatus

Gets the current port status.

DriverKit 19.0+

``` source
kern_return_t GetPortStatus(uint32_t * portStatus);
```

## Parameters 

`portStatus`  

A pointer to a variable. On return, the variable contains the port status. For a list of possible port status values, see tIOUSBHostPortStatus.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Configuring the Interface

GetFrameNumber

Gets the current frame number of the USB controller.

SelectAlternateSetting

Selects an alternative setting for this interface.

GetIdlePolicy

Gets the current idle suspend timeout for the interface.

SetIdlePolicy

Sets the desired idle suspend timeout for the interface.

tIOUSBHostPortStatus

Constants indicating the state of a port.

