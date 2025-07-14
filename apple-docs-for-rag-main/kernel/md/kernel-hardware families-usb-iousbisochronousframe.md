

- Kernel
- Hardware Families
- USB
-  IOUSBIsochronousFrame 

Structure

# IOUSBIsochronousFrame

A structure representing a single frame in an isochronous transfer.

macOS 10.15+

``` source
typedef struct IOUSBIsochronousFrame {
    ...
} IOUSBIsochronousFrame;
```

## Topics

### Getting the Frame Properties

status

The completion status for this individual frame.

requestCount

The number of bytes to transfer for this frame.

completeCount

The number of bytes that the system actually transferred for this frame.

reserved

Reserved for future use.

timeStamp

The frame’s observed completion time.

## See Also

### USB Specifications

USB Device Descriptors

Structures and functions for working with device descriptors.

Additional Specifications

Structures related to hubs, devices, and endpoints.

