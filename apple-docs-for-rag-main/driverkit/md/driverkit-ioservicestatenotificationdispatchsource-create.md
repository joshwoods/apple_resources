

- DriverKit
- IOServiceStateNotificationDispatchSource
-  Create 

Static Method

# Create

DriverKitiOSiPadOSmacOS

``` source
static kern_return_t Create(IOService * service, OSArray * items, IODispatchQueue * queue, IOServiceStateNotificationDispatchSource * * source);
```

## Return Value

kIOReturnSuccess on success. See `IOReturn.h` for error codes.

