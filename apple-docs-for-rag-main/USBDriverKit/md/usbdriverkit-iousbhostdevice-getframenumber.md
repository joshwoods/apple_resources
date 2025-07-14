

- USBDriverKit
- IOUSBHostDevice
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

### Getting Device Information

GetAddress

Returns the address of the device.

GetSpeed

Retrieves the device’s operational speed.

GetPortStatus

Returns the current port status of the device.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

tIOUSBHostPortStatus

Constants indicating the state of a port.

tIOUSBHostPortType

Constants indicating a port’s type.

