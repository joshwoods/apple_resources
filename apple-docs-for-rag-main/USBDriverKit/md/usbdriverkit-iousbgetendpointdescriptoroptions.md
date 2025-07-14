

- USBDriverKit
-  IOUSBGetEndpointDescriptorOptions 

Enumeration

# IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

DriverKit 19.0+

``` source
enum IOUSBGetEndpointDescriptorOptions : unsigned int;
```

## Topics

### Getting the Descriptor Options

kIOUSBGetEndpointDescriptorOriginal

The original descriptor used to create the pipe.

kIOUSBGetEndpointDescriptorCurrentPolicy

The descriptor controlling the current endpoint policy.

## See Also

### Getting the Endpoint Descriptors

GetDescriptors

Retrieves the endpoint descriptors associated with this pipe.

IOUSBStandardEndpointDescriptors

Encapsulates the descriptors for a single endpoint.

