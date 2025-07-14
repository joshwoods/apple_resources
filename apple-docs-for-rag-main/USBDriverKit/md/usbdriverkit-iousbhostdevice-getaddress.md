

- USBDriverKit
- IOUSBHostDevice
-  GetAddress 

Instance Method

# GetAddress

Returns the address of the device.

DriverKit 19.0+

``` source
kern_return_t GetAddress(uint8_t * address) const;
```

## Parameters 

`address`  

A pointer to a variable. On output, the variable contains the device’s address.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Getting Device Information

GetSpeed

Retrieves the device’s operational speed.

GetFrameNumber

Gets the current frame number of the USB controller.

GetPortStatus

Returns the current port status of the device.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

tIOUSBHostPortStatus

Constants indicating the state of a port.

tIOUSBHostPortType

Constants indicating a port’s type.

