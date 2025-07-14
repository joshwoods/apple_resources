

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSB3HubDescriptor 

Structure

# IOUSB3HubDescriptor

A structure that defines the descriptor for a USB 3.0 hub.

macOS 10.8+

``` source
typedef struct IOUSB3HubDescriptor {
    ...
} IOUSB3HubDescriptor;
```

## Topics

### Instance Properties

characteristics

hubCurrent

hubDelay

hubHdrDecLat

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

IOUSBHubDescriptor

A structure that defines the descriptor for a USB hub.

IOUSBHubPortReEnumerateParam

A structure for USB hub port reenumeration.

