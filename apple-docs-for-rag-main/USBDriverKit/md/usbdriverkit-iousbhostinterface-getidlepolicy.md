

- USBDriverKit
- IOUSBHostInterface
-  GetIdlePolicy 

Instance Method

# GetIdlePolicy

Gets the current idle suspend timeout for the interface.

DriverKit 19.0+

``` source
kern_return_t GetIdlePolicy(uint32_t * deviceIdleTimeout);
```

## Parameters 

`deviceIdleTimeout`  

A pointer to a variable. On return, the variable contains the amount of time, in milliseconds, to wait after all pipes are idle before suspending the device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Configuring the Interface

GetFrameNumber

Gets the current frame number of the USB controller.

GetPortStatus

Gets the current port status.

SelectAlternateSetting

Selects an alternative setting for this interface.

SetIdlePolicy

Sets the desired idle suspend timeout for the interface.

tIOUSBHostPortStatus

Constants indicating the state of a port.

