

- USBDriverKit
-  tIOUSBDescriptorType 

Enumeration

# tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

DriverKit 19.0+

``` source
enum tIOUSBDescriptorType : unsigned int;
```

## Overview

When you fetch descriptors from a USB device, the data includes a one-byte value that indicates the type of the descriptor. Use these constants to determine the type.

For detailed information about the descriptor types, see Table 9-5 of the USB 2.0 specification and Table 9-6 of the USB 3.0 specification at https://www.usb.org/.

## Topics

### Getting the Descriptor Type

kIOUSBDescriptorTypeDevice

The type for a device descriptor.

kIOUSBDescriptorTypeConfiguration

The type for a configuration descriptor.

kIOUSBDescriptorTypeString

The type for a string descriptor.

kIOUSBDescriptorTypeInterface

The type for an interface descriptor.

kIOUSBDescriptorTypeEndpoint

The type for an endpoint descriptor.

kIOUSBDescriptorTypeDeviceQualifier

The type for a device qualifier descriptor.

kIOUSBDescriptorTypeOtherSpeedConfiguration

The type for an other speed configuration descriptor.

kIOUSBDescriptorTypeInterfacePower

The type for an interface power descriptor.

kIOUSBDescriptorTypeOTG

The type for an on-the-go descriptor.

kIOUSBDescriptorTypeDebug

The type for a debug descriptor.

kIOUSBDescriptorTypeInterfaceAssociation

The type for an interface association descriptor.

kIOUSBDescriptorTypeBOS

The type for a binary object store descriptor.

kIOUSBDescriptorTypeDeviceCapability

The type for a capability descriptor.

kIOUSBDecriptorTypeHID

The type for a human interaction device descriptor.

kIOUSBDecriptorTypeReport

The type for a report descriptor.

kIOUSBDescriptorTypePhysical

The type for a physical descriptor.

kIOUSBDescriptorTypeHub

The type for a hub descriptor.

kIOUSBDescriptorTypeSuperSpeedHub

The type for a super-speed hub descriptor.

kIOUSBDescriptorTypeSuperSpeedUSBEndpointCompanion

The type for a super-speed endpoint companion descriptor.

kIOUSBDescriptorTypeSuperSpeedPlusIsochronousEndpointCompanion

The type for a super-speed plus isochronous endpoint companion descriptor.

## See Also

### Descriptor Fundamentals

IOUSBDescriptorHeader

The base descriptor header.

IOUSBDescriptor

The base descriptor type.

tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

