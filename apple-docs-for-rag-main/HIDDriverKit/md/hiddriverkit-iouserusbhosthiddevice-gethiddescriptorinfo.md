

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  getHIDDescriptorInfo 

Instance Method

# getHIDDescriptorInfo

DriverKitmacOS

``` source
kern_return_t getHIDDescriptorInfo(uint8_t type, const IOUSBHostHIDDescriptorInfo * * info, uint8_t * index);
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Configuring Private Settings

initPipes

CompleteZLP

copyStringAtIndex

