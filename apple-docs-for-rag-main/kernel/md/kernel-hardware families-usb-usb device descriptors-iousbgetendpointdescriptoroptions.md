

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBGetEndpointDescriptorOptions 

# IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

macOS 10.15+

``` source
enum IOUSBGetEndpointDescriptorOptions : unsigned int {
    ...
};
```

## Topics

### Getting the Options

kIOUSBGetEndpointDescriptorOriginal

The original descriptor that the system uses to create the pipe.

kIOUSBGetEndpointDescriptorCurrentPolicy

The descriptor controlling the current endpoint policy.

## See Also

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

