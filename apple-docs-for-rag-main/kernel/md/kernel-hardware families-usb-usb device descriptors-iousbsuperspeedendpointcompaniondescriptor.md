

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBSuperSpeedEndpointCompanionDescriptor 

Type Alias

# IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB endpoint companion.

macOS 10.7+

``` source
typedef struct IOUSBSuperSpeedEndpointCompanionDescriptor IOUSBSuperSpeedEndpointCompanionDescriptor;
```

## Discussion

For more information about this descriptor type, see USB 3.2, 9.6.7.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bMaxBurst

The maximum number of packets the endpoint can send or receive as part of a burst.

bmAttributes

A bitmap encoding of supported device-level features.

wBytesPerInterval

The total number of bytes this endpoint transfers every service interval.

## See Also

### USB Descriptors

IOUSBStringDescriptor

The structure for storing a string descriptor.

IOUSBStringDescriptorPtr

A pointer to a string descriptor structure.

IOUSBSuperSpeedEndpointCompanionDescriptorPtr

A pointer to a SuperSpeed USB endpoint companion descriptor.

IOUSBSuperSpeedHubDescriptor

A structure that defines the descriptor for a SuperSpeed USB hub.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptorPtr

A pointer to a SuperSpeedPlus isochronous USB endpoint companion descriptor.

### Related Documentation

IOUSBSuperSpeedEndpointCompanionDescriptor

