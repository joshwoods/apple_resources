

- USBDriverKit
- IOUSBHostInterface
-  GetFrameNumber 

Instance Method

# GetFrameNumber

Gets the current frame number of the USB controller.

DriverKit 19.0+

``` source
kern_return_t GetFrameNumber(uint64_t * frameNumber, uint64_t * theTime);
```

## Parameters 

`frameNumber`  

A pointer to a variable. On return, this variable contains the current frame number.

`theTime`  

A pointer to a variable. On return, this variable contains the current time.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method returns the current frame number of the USB controller, omitting the microframe. Use this information to schedule future isochronous requests.

## See Also

### Configuring the Interface

GetPortStatus

Gets the current port status.

SelectAlternateSetting

Selects an alternative setting for this interface.

GetIdlePolicy

Gets the current idle suspend timeout for the interface.

SetIdlePolicy

Sets the desired idle suspend timeout for the interface.

tIOUSBHostPortStatus

Constants indicating the state of a port.

