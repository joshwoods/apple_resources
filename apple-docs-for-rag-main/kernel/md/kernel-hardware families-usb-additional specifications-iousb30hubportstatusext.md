

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSB30HubPortStatusExt 

# IOUSB30HubPortStatusExt

A structure that represents an extension to the USB 3.0 hub port status.

macOS 10.15+

``` source
struct IOUSB30HubPortStatusExt {
    ...
};
```

## Discussion

For information about this type, see USB 3.2, 10.16.2.6.

## Topics

### Getting the Properties

dwExtPortStatus

The extended port status bits.

wPortChange

The port status change bits.

wPortStatus

The port status field bits.

## See Also

### Hub Port Status Requests

IOUSBHubPortStatus

A structure that contains the USB hub port status.

IOUSBHubStatusPtr

A pointer to a USB hub status structure.

IOUSBHubStatus

A structure that represents the USB hub status.

