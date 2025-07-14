

- Kernel
- IOKit Fundamentals
-  DriverOSRuntime 

Structure

# DriverOSRuntime

macOS 10.0+

``` source
typedef struct DriverOSRuntime {
    ...
} DriverOSRuntime;
```

## Topics

### Instance Properties

driverDescReserved

driverName

driverRuntime

## See Also

### Utilities

IOServiceOrdering

IOFixedDivide

IOFixedMultiply

IOAlignmentToSize

IOSizeToAlignment

OSSynchronizeIO

The OSSynchronizeIO routine ensures orderly load and store operations to noncached memory mapped I/O devices.

DriverDescription

DriverOSService

DriverServiceInfo

DriverType

