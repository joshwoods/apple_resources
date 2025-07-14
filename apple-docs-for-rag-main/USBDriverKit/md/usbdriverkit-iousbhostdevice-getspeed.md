

- USBDriverKit
- IOUSBHostDevice
-  GetSpeed 

Instance Method

# GetSpeed

Retrieves the device’s operational speed.

DriverKit 19.0+

``` source
kern_return_t GetSpeed(uint8_t * speed) const;
```

## Parameters 

`speed`  

A pointer to a variable. On output, the variable contains the operational speed of the device. For a list of possible values, see tIOUSBHostConnectionSpeed.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Getting Device Information

GetAddress

Returns the address of the device.

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

