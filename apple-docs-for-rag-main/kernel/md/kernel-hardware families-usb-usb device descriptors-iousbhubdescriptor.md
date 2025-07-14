

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBHubDescriptor 

Structure

# IOUSBHubDescriptor

A structure that defines the descriptor for a USB hub.

macOS 10.8+

``` source
typedef struct IOUSBHubDescriptor {
    ...
} IOUSBHubDescriptor;
```

## Topics

### Instance Properties

characteristics

hubCurrent

hubType

length

numPorts

powerOnToGood

pwrCtlPortFlags

removablePortFlags

## See Also

### Hub Descriptors

IOUSB20HubDescriptor

A structure that defines the descriptor for a USB 2.0 hub.

IOUSB3HubDescriptor

A structure that defines the descriptor for a USB 3.0 hub.

IOUSBHubPortReEnumerateParam

A structure for USB hub port reenumeration.

