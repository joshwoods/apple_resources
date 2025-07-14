

- Kernel
- IOKit Fundamentals
-  OSSynchronizeIO 

Function

# OSSynchronizeIO

The OSSynchronizeIO routine ensures orderly load and store operations to noncached memory mapped I/O devices.

macOS 10.0+

``` source
void OSSynchronizeIO(void);
```

## Discussion

The OSSynchronizeIO routine ensures orderly load and store operations to noncached memory mapped I/O devices. It executes the eieio instruction on PowerPC processors.

## See Also

### Utilities

IOServiceOrdering

IOFixedDivide

IOFixedMultiply

IOAlignmentToSize

IOSizeToAlignment

DriverDescription

DriverOSRuntime

DriverOSService

DriverServiceInfo

DriverType

