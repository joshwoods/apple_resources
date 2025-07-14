

- Kernel
- IOKit Fundamentals
-  IOServiceOrdering 

Function

# IOServiceOrdering

macOS 10.0+

``` source
SInt32 IOServiceOrdering(const OSMetaClassBase *inObj1, const OSMetaClassBase *inObj2, void *ref);
```

## See Also

### Utilities

IOFixedDivide

IOFixedMultiply

IOAlignmentToSize

IOSizeToAlignment

OSSynchronizeIO

The OSSynchronizeIO routine ensures orderly load and store operations to noncached memory mapped I/O devices.

DriverDescription

DriverOSRuntime

DriverOSService

DriverServiceInfo

DriverType

