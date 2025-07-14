

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor 

Type Alias

# IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

macOS 10.15+

``` source
typedef struct IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor;
```

## Discussion

See USB 3.2, 9.6.8 for more information.

## Topics

### Instance Properties

bDescriptorType

bLength

dwBytesPerInterval

wReserved

## See Also

### USB Descriptors

IOUSBStringDescriptor

The structure for storing a string descriptor.

IOUSBStringDescriptorPtr

A pointer to a string descriptor structure.

IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB endpoint companion.

IOUSBSuperSpeedEndpointCompanionDescriptorPtr

A pointer to a SuperSpeed USB endpoint companion descriptor.

IOUSBSuperSpeedHubDescriptor

A structure that defines the descriptor for a SuperSpeed USB hub.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptorPtr

A pointer to a SuperSpeedPlus isochronous USB endpoint companion descriptor.

