

- Kernel
- Hardware Families
- USB
-  USB Device Descriptors 

API Collection

# USB Device Descriptors

Structures and functions for working with device descriptors.

## Topics

### Descriptor Fundamentals

IOUSBDescriptorHeader

The base descriptor header.

IOUSBDescriptor

The base descriptor type.

tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

IOUSBDescriptorHeaderPtr

A pointer to a USB descriptor header.

### Device Descriptors

IOUSBDeviceDescriptor

The structure for storing a USB device descriptor.

IOUSBDeviceDescriptorPtr

A pointer to a USB device descriptor.

IOUSBDeviceQualifierDescriptor

The structure for describing a high-speed capable USB device.

IOUSBDeviceQualifierDescriptorPtr

A pointer to a qualifier descriptor.

### Configuration Descriptors

IOUSBConfigurationDescriptor

The structure for storing a USB configuration descriptor.

IOUSBConfigurationDescHeader

The header of a configuration descriptor.

IOUSBConfigurationDescriptorPtr

A pointer to a configuration descriptor.

IOUSBConfigurationDescHeaderPtr

A pointer to a configuration descriptor header.

### Interface Descriptors

IOUSBInterfaceDescriptor

A descriptor for a specific interface of a USB device.

IOUSBInterfaceDescriptorPtr

A pointer to a USB interface descriptor.

IOUSBInterfaceAssociationDescriptor

The descriptor that associates multiple interfaces to the same function.

IOUSBInterfaceAssociationDescriptorPtr

A pointer to a USB interface association descriptor.

### Endpoint Descriptors

IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

IOUSBStandardEndpointDescriptors

A container for descriptors for a single endpoint.

IOUSBEndpointDescriptorPtr

A pointer to the endpoint descriptor.

IOUSBEndpointProperties

A structure that holds USB endpoint properties.

IOUSBEndpointPropertiesPtr

A pointer to an endpoint properties object.

IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

### Capability Descriptors

IOUSBPlatformCapabilityDescriptor

The structure for the platform capability descriptor.

IOUSBPlatformCapabilityDescriptorPtr

A pointer to a USB platform capability descriptor.

IOUSBDeviceCapabilityBillboard

The structure for the billboard device capability.

IOUSBDeviceCapabilityBillboardAltConfig

The structure for the billboard alternative configuration device capability.

IOUSBDeviceCapabilityBillboardAltConfigCompatibility

The structure for the billboard alternative configuration compatibility device capability.

IOUSBDeviceCapabilityBillboardAltConfigPtr

A pointer to a USB device capability billboard alternative configuration structure.

IOUSBDeviceCapabilityBillboardAltMode

The structure for the billboard alternative mode device capability.

IOUSBDeviceCapabilityBillboardAltModePtr

A pointer to a USB device capability billboard alternative mode structure.

IOUSBDeviceCapabilityBillboardPtr

A pointer to a USB device capability billboard object.

IOUSBDeviceCapabilityContainerID

The structure for the container ID device capability.

IOUSBDeviceCapabilityContainerIDPtr

A pointer to a USB device capability container ID.

IOUSBDeviceCapabilityDescriptorHeader

The device capability descriptor header.

IOUSBDeviceCapabilityDescriptorHeaderPtr

A pointer to a device capability descriptor header.

IOUSBDeviceCapabilitySuperSpeedPlusUSB

The structure for the SuperSpeedPlus USB device capability.

IOUSBDeviceCapabilitySuperSpeedPlusUSBPtr

A pointer to a SuperSpeedPlus USB device capability structure.

IOUSBDeviceCapabilitySuperSpeedUSB

The structure for the SuperSpeed USB device capability.

IOUSBDeviceCapabilitySuperSpeedUSBPtr

A pointer to a SuperSpeed USB device capability structure.

IOUSBDeviceCapabilityUSB2Extension

The structure for the USB 2.0 extension device capability.

IOUSBDeviceCapabilityUSB2ExtensionPtr

A pointer to a USB 2.0 extension device capability structure.

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

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptorPtr

A pointer to a SuperSpeedPlus isochronous USB endpoint companion descriptor.

### HID Descriptors

IOUSBHIDData

Data related to the mouse and keyboard.

IOUSBHIDDataPtr

A pointer to a structure related to mouse and keyboard data.

IOUSBHIDDescriptor

A structure that defines the USB HID descriptor.

IOUSBHIDDescriptorPtr

A pointer to a structure that defines the USB HID descriptor.

IOUSBHIDReportDesc

A structure that defines the USB HID report descriptor header.

IOUSBHIDReportDescPtr

A pointer to a structure that defines the USB HID report descriptor header.

### Device Firmware Update Descriptors

IOUSBDFUDescriptor

A structure that defines the USB device firmware update descriptor.

IOUSBDFUDescriptorPtr

A pointer to a structure that defines the USB device firmware update descriptor.

### BOS Descriptors

IOUSBBOSDescriptor

The structure for storing a binary object store (BOS) descriptor.

IOUSBBOSDescriptorPtr

A pointer to a structure for storing a binary object store (BOS) descriptor.

### Hub Descriptors

IOUSB20HubDescriptor

A structure that defines the descriptor for a USB 2.0 hub.

IOUSB3HubDescriptor

A structure that defines the descriptor for a USB 3.0 hub.

IOUSBHubDescriptor

A structure that defines the descriptor for a USB hub.

IOUSBHubPortReEnumerateParam

A structure for USB hub port reenumeration.

## See Also

### USB Specifications

IOUSBIsochronousFrame

A structure representing a single frame in an isochronous transfer.

Additional Specifications

Structures related to hubs, devices, and endpoints.

