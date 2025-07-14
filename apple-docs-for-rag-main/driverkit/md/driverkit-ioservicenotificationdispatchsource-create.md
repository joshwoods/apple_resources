

- DriverKit
- IOServiceNotificationDispatchSource
-  Create 

Static Method

# Create

DriverKitiOSiPadOSmacOS

``` source
static kern_return_t Create(OSDictionary * matching, uint64_t options, IODispatchQueue * queue, IOServiceNotificationDispatchSource * * notification);
```

## Return Value

kIOReturnSuccess on success. See `IOReturn.h` for error codes.

