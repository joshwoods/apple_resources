

- USBDriverKit
- IOUSBHostPipe
-  GetDeviceAddress 

Instance Method

# GetDeviceAddress

Retrieves the address of the device.

DriverKit 19.0+

``` source
kern_return_t GetDeviceAddress(uint8_t * address) const;
```

## Parameters 

`address`  

A pointer to a variable. On output, the variable contains the device’s address.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Getting the Device Attributes

GetSpeed

Retrieves the device’s operational speed.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

