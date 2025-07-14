

- USBDriverKit
- IOUSBHostInterface
-  CopyPipe 

Instance Method

# CopyPipe

Returns the pipe for the specified endpoint address.

DriverKit 19.0+

``` source
kern_return_t CopyPipe(uint8_t address, IOUSBHostPipe * * pipe);
```

## Parameters 

`address`  

The address of the pipe you want. Get the address for a specific pipe from the bEndpointAddress field of the appropriate IOUSBEndpointDescriptor structure.

`pipe`  

A variable in which to store the IOUSBHostPipe object. It’s your responsibility to release this object when you finish using it.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

If the specified pipe doesn’t exist yet, but is part of the interface, this method creates the pipe before returning it.

