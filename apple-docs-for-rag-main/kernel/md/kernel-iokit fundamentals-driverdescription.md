

- Kernel
- IOKit Fundamentals
-  DriverDescription 

Structure

# DriverDescription

macOS 10.0+

``` source
typedef struct DriverDescription {
    ...
} DriverDescription;
```

## Topics

### Instance Properties

driverDescSignature

driverDescVersion

driverOSRuntimeInfo

driverServices

driverType

## See Also

### Utilities

IOServiceOrdering

IOFixedDivide

IOFixedMultiply

IOAlignmentToSize

IOSizeToAlignment

OSSynchronizeIO

The OSSynchronizeIO routine ensures orderly load and store operations to noncached memory mapped I/O devices.

DriverOSRuntime

DriverOSService

DriverServiceInfo

DriverType

