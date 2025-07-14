

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBHubStatus 

Structure

# IOUSBHubStatus

A structure that represents the USB hub status.

macOS 10.8+

``` source
typedef struct IOUSBHubStatus {
    ...
} IOUSBHubStatus;
```

## Overview

Use this structure when obtaining the port status and change flags with GetPortStatus.

## Topics

### Instance Properties

changeFlags

statusFlags

## See Also

### Hub Port Status Requests

IOUSB30HubPortStatusExt

A structure that represents an extension to the USB 3.0 hub port status.

IOUSBHubPortStatus

A structure that contains the USB hub port status.

IOUSBHubStatusPtr

A pointer to a USB hub status structure.

### Related Documentation

