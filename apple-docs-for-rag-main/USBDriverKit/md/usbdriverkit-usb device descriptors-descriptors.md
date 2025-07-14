

- USBDriverKit
-  USB Device Descriptors 

API Collection

# USB Device Descriptors

Determine the capabilities and configuration of a device using descriptors from the USB specification.

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

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

### Device Descriptors

IOUSBDeviceDescriptor

The structure for storing a USB device descriptor.

IOUSBDeviceQualifierDescriptor

The structure for storing a USB device qualifier descriptor.

Apple’s Vendor ID

Apple’s vendor ID, assigned by the USB-IF.

### Configuration Descriptors

IOUSBConfigurationDescriptor

The structure for storing a USB configuration descriptor.

IOUSBConfigurationDescHeader

The header of a configuration descriptor.

Power Configuration Settings

Constants for configuring the power settings.

### Interface Descriptors

IOUSBInterfaceDescriptor

A descriptor for a specific interface of a USB device.

IOUSBInterfaceAssociationDescriptor

The USB Interface Association Descriptor.

### Endpoint Descriptors

IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB Endpoint Companion.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus Isochronous USB Endpoint Companion.

tIOUSBEndpointType

Constants describing the types of endpoints.

Endpoint Attributes

Constants for endpoint attributes.

SuperSpeed USB Endpoint Descriptor Options

Constants for super-speed endpoint attributes.

tIOUSBEndpointDirection

The direction of data transfers on an endpoint.

tIOUSBEndpointSynchronizationType

Constants for the endpoint synchronization types.

tIOUSBEndpointUsageType

Constants for the endpoint usage types.

tIOUSBLanguageID

Constants for the USB language identifiers.

### String Descriptor

IOUSBStringDescriptor

The structure for storing a string descriptor.

### Capability Descriptors

IOUSBBOSDescriptor

The structure for storing a binary object store (BOS) descriptor.

IOUSBDeviceCapabilityDescriptorHeader

The device capability descriptor header.

IOUSBDeviceCapabilityBillboard

The structure for the billboard device capability.

IOUSBDeviceCapabilityBillboardAltConfig

The structure for the billboard alternative configuration device capability.

IOUSBDeviceCapabilityBillboardAltConfigCompatibility

The structure for the billboard alternative configuration compatibility device capability.

IOUSBDeviceCapabilityBillboardAltMode

The structure for the billboard alternative mode device capability.

IOUSBDeviceCapabilityContainerID

The structure for the container ID device capability.

IOUSBDeviceCapabilitySuperSpeedUSB

The structure for the super-speed USB device capability.

IOUSBDeviceCapabilitySuperSpeedPlusUSB

The structure for the super-speed plus USB device capability.

IOUSBDeviceCapabilityUSB2Extension

The structure for the USB 2 extension device capability.

IOUSBPlatformCapabilityDescriptor

The structure for the platform capability descriptor.

tIOUSBDeviceCapabilityType

Constants for the device capability types.

SuperSpeed Device Capabilities

Constants for configuring super-speed device capabilities.

SuperSpeedPlus Device Capabilities

Constants for configuring super-speed plus device capabilities.

### USB Descriptors

IOUSB20HubDescriptor

A structure that defines the descriptor for a USB hub.

IOUSBSuperSpeedHubDescriptor

A structure that defines the descriptor for a Super Speed USB hub.

SuperSpeed Hub Characteristics

Constants for specifying super-speed hub characteristics.

UASPipeDescriptor

A structure that defines the Mass Storage Specific UAS pipe usage descriptor.

### HID Descriptors

IOUSBHIDDescriptor

A structure that defines the USB HID Descriptor.

IOUSBHIDReportDesc

A structure that defines the USB HID Report Descriptor header.

### Firmware Update Descriptor

IOUSBDFUDescriptor

A structure that defines the USB device firmware update descriptor.

## See Also

### USB Specifications

Additional Specifications

Request information from a device and get hardware and timing information.

Registry Property Names

Search for specific keys in the device registry.

Utilities

Manipulate bit structures and convert integers between device- and platform-native formats.

