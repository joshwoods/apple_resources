

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBSuperSpeedHubDescriptor 

Type Alias

# IOUSBSuperSpeedHubDescriptor

A structure that defines the descriptor for a SuperSpeed USB hub.

macOS 10.15+

``` source
typedef struct IOUSBSuperSpeedHubDescriptor IOUSBSuperSpeedHubDescriptor;
```

## Discussion

For more information about this descriptor type, see USB 3.2, 10.15.2.1.

## Topics

### Instance Properties

bDescriptorType

bHubControllerCurrent

bHubDecodeLatency

bLength

bNumberPorts

bPowerOnToPowerGood

deviceRemovable

wHubCharacteristics

wHubDelay

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

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptorPtr

A pointer to a SuperSpeedPlus isochronous USB endpoint companion descriptor.

