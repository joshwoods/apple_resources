

- USBDriverKit
- IOUSBHostInterface
-  CopyDevice 

Instance Method

# CopyDevice

Returns the host device object that contains this interface.

DriverKit 19.0+

``` source
kern_return_t CopyDevice(IOUSBHostDevice * * device);
```

## Parameters 

`device`  

A variable in which to store the IOUSBHostDevice object. It’s your responsibility to release this object when you finish using it.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

