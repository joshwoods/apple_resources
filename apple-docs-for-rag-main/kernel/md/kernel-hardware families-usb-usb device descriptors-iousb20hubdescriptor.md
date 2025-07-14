

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSB20HubDescriptor 

Type Alias

# IOUSB20HubDescriptor

A structure that defines the descriptor for a USB 2.0 hub.

macOS 10.15+

``` source
typedef struct IOUSB20HubDescriptor IOUSB20HubDescriptor;
```

## Discussion

For more information about this descriptor type, see USB 2.0, 11.23.2.1.

## Topics

### Instance Properties

bDescriptorType

bHubControllerCurrent

bLength

bNumberPorts

bPowerOnToPowerGood

deviceRemovable

reserved

wHubCharacteristics

## See Also

### Hub Descriptors

IOUSB3HubDescriptor

A structure that defines the descriptor for a USB 3.0 hub.

IOUSBHubDescriptor

A structure that defines the descriptor for a USB hub.

IOUSBHubPortReEnumerateParam

A structure for USB hub port reenumeration.

