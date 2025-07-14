

- USBDriverKit
- IOUSBHostDevice
-  Descriptor Utilities 

API Collection

# Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

## Topics

### Configuration Descriptors

IOUSBGetNextDescriptor

Gets the next descriptor in a configuration descriptor.

IOUSBGetNextDescriptorWithType

Finds the next descriptor matching a given type within a configuration descriptor.

IOUSBGetNextAssociatedDescriptor

Gets the next descriptor in the specified configuration descriptor that belongs to another container descriptor.

IOUSBGetNextAssociatedDescriptorWithType

Finds the next descriptor matching a specific type within a configuration descriptor that belongs to another container descriptor.

IOUSBGetConfigurationMaxPowerMilliAmps

Extracts the maximum bus current a configuration descriptor requires.

### Interface Descriptors

IOUSBGetNextInterfaceDescriptor

Finds the next interface descriptor in a configuration descriptor.

IOUSBGetNextInterfaceAssociationDescriptor

Finds the next interface association descriptor in a configuration descriptor.

### Endpoint Descriptors

IOUSBGetNextEndpointDescriptor

Finds the next endpoint descriptor associated with an interface descriptor.

IOUSBGetEndpointAddress

Extracts the direction and number of an endpoint from an endpoint descriptor.

IOUSBGetEndpointBurstSize

Extracts the burst size from endpoint descriptors.

IOUSBGetEndpointDirection

Extracts the direction of an endpoint from an endpoint descriptor.

IOUSBGetEndpointIntervalEncodedMicroframes

Extracts the interval of an endpoint descriptor.

IOUSBGetEndpointIntervalFrames

Extracts the interval of an endpoint descriptor.

IOUSBGetEndpointIntervalMicroframes

Extracts the interval of an endpoint descriptor.

IOUSBGetEndpointMaxPacketSize

Extracts the maximum packet size from an endpoint descriptor.

IOUSBGetEndpointMaxStreams

Extracts the number of streams an endpoint supports.

IOUSBGetEndpointMaxStreamsEncoded

Extracts the number of streams an endpoint supports.

IOUSBGetEndpointMult

Extracts the mult count from endpoint descriptors.

IOUSBGetEndpointNumber

Extracts the number of an endpoint from an endpoint descriptor.

IOUSBGetEndpointType

Extracts the type of an endpoint from an endpoint descriptor.

### BOS Descriptors

IOUSBGetNextCapabilityDescriptor

Gets the next device capability descriptor in a BOS descriptor.

IOUSBGetNextCapabilityDescriptorWithType

Finds the next descriptor matching a given type within a BOS descriptor.

IOUSBGetSuperSpeedDeviceCapabilityDescriptor

Finds the first SuperSpeed device capability descriptor in a BOS descriptor.

IOUSBGetSuperSpeedPlusDeviceCapabilityDescriptor

Finds the first SuperSpeed Plus device capability descriptor in a BOS descriptor.

IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor

Finds the first USB 2.0 extension capability descriptor in a BOS descriptor.

IOUSBGetContainerIDDescriptor

Finds the first Container ID capability descriptor in a BOS descriptor.

IOUSBGetPlatformCapabilityDescriptor

Finds the first platform capability descriptor in a BOS descriptor.

IOUSBGetBillboardDescriptor

Finds the first billboard capability descriptor in a BOS descriptor.

## See Also

### Getting the Device Descriptors

CopyCapabilityDescriptors

Returns the device’s capability descriptors.

CopyConfigurationDescriptor

Returns the configuration descriptor with the specified index.

CopyConfigurationDescriptor

Returns the currently selected configuration descriptor.

CopyConfigurationDescriptorWithValue

Returns the configuration descriptor with the specified configuration value.

CopyDeviceDescriptor

Returns the device descriptor.

CopyStringDescriptor

Returns a string descriptor from the device.

CopyStringDescriptor

Returns a string descriptor from the device.

CopyDescriptor

Retrieves any type of descriptor from the cache or the device.

tIOUSBDeviceRequestTypeValue

Constants indicating the type of request to make from a device.

tIOUSBDeviceRequestRecipientValue

Constants indicating the type of object that receives the results of a request.

