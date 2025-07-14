

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  tIOUSBDescriptorType 

Type Alias

# tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

macOS 10.15+

``` source
typedef enum tIOUSBDescriptorType tIOUSBDescriptorType;
```

## Discussion

When you fetch descriptors from a USB device, the data includes a one-byte value that indicates the type of the descriptor. Use these constants to determine the type.

For detailed information about the descriptor types, see USB 3.2, 9.4.

## Topics

### Getting the Descriptor Type

kIOUSBDecriptorTypeHID

The type for a human interaction device descriptor.

kIOUSBDecriptorTypeReport

The type for a report descriptor.

kIOUSBDescriptorTypePhysical

The type for a physical descriptor.

### Constants

kIOUSBDescriptorTypeBOS

kIOUSBDescriptorTypeConfiguration

kIOUSBDescriptorTypeDebug

kIOUSBDescriptorTypeDevice

kIOUSBDescriptorTypeDeviceCapability

kIOUSBDescriptorTypeDeviceQualifier

kIOUSBDescriptorTypeEndpoint

kIOUSBDescriptorTypeHub

kIOUSBDescriptorTypeInterface

kIOUSBDescriptorTypeInterfaceAssociation

kIOUSBDescriptorTypeInterfacePower

kIOUSBDescriptorTypeOTG

kIOUSBDescriptorTypeOtherSpeedConfiguration

kIOUSBDescriptorTypeString

kIOUSBDescriptorTypeSuperSpeedHub

kIOUSBDescriptorTypeSuperSpeedPlusIsochronousEndpointCompanion

kIOUSBDescriptorTypeSuperSpeedUSBEndpointCompanion

## See Also

### Descriptor Fundamentals

IOUSBDescriptorHeader

The base descriptor header.

IOUSBDescriptor

The base descriptor type.

tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

IOUSBDescriptorHeaderPtr

A pointer to a USB descriptor header.

