

- USBDriverKit
-  tIOUSBDescriptorSize 

Enumeration

# tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

DriverKit 19.0+

``` source
enum tIOUSBDescriptorSize : unsigned int;
```

## Topics

### Getting the Descriptor Size

kIOUSBDescriptorHeaderSize

The size of a descriptor header.

kIOUSBDescriptorSizeDevice

The size of a device descriptor.

kIOUSBDescriptorSizeConfiguration

The size of a configuration descriptor.

kIOUSBDescriptorSizeInterface

The size of an interface descriptor.

kIOUSBDescriptorSizeEndpoint

The size of an endpoint descriptor.

kIOUSBDescriptorSizeStringMinimum

The minimum size of a string descriptor.

kIOUSBDescriptorSizeStringMaximum

The maximum size of a string descriptor.

kIOUSBDescriptorSizeDeviceQualifier

The size of a device qualifier descriptor.

kIOUSBDescriptorSizeInterfaceAssociation

The size of an interface association descriptor.

kIOUSBDescriptorSizeBOS

The size of a binary object store descriptor.

kIOUSBDescriptorSizeDeviceCapability

The size of a device capability descriptor.

kIOUSBDescriptorSizeUSB20ExtensionCapability

The size of a USB 2.0 extension capability descriptor.

kIOUSBDescriptorSizeSuperSpeedUSBDeviceCapability

The size of a super-speed device capability descriptor.

kIOUSBDescriptorSizeContainerIDCapability

The size of a container ID capability descriptor.

kIOUSBDescriptorSizeHubMinimum

The minimum size of a hub descriptor.

kIOUSBDescriptorSizeHubMaximum

The maximum size of a hub descriptor.

kIOUSBDescriptorSizeSuperSpeedHub

The size of a super-speed hub descriptor.

kIOUSBDescriptorSizeSuperSpeedUSBEndpointCompanion

The size of a super-speed endpoint companion descriptor.

kIOUSBDescriptorSizeSuperSpeedPlusIsochronousEndpointCompanion

The size of a super-speed plus isochronous endpoint companion descriptor.

kIOUSBDescriptorSizeBillboardDeviceMinimum

The minimum size of a billboard descriptor.

kIOUSBDescriptorSizeBillboardDeviceMaximum

The maximum size of a billboard descriptor.

kIOUSBDescriptorSizePlatformECIDCapability

The size of a platform ECID capability descriptor.

kIOUSBDescriptorSizePlatformCapability

The size of a platform capability descriptor.

## See Also

### Descriptor Fundamentals

IOUSBDescriptorHeader

The base descriptor header.

IOUSBDescriptor

The base descriptor type.

tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

