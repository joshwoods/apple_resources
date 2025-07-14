

- USBDriverKit
- IOUSBHostDevice
-  GetPortStatus 

Instance Method

# GetPortStatus

Returns the current port status of the device.

DriverKit 19.0+

``` source
kern_return_t GetPortStatus(uint32_t * portStatus);
```

## Parameters 

`portStatus`  

A pointer to a variable. On output, the variable contains the port status. For a list of possible values, see tIOUSBHostPortStatus.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Getting Device Information

GetAddress

Returns the address of the device.

GetSpeed

Retrieves the device’s operational speed.

GetFrameNumber

Gets the current frame number of the USB controller.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

tIOUSBHostPortStatus

Constants indicating the state of a port.

tIOUSBHostPortType

Constants indicating a port’s type.

