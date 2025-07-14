

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBEndpointDescriptor 

Type Alias

# IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

macOS 10.0+

``` source
typedef struct IOUSBEndpointDescriptor IOUSBEndpointDescriptor;
```

## Discussion

A descriptor for a USB endpoint. See USB 3.2, 9.6.6.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bEndpointAddress

The address of the endpoint.

bmAttributes

The attributes of the endpoint.

wMaxPacketSize

The maximum packet size that the endpoint supports.

bInterval

The interval to use when polling the endpoint for data transfers.

## See Also

### Endpoint Descriptors

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

### Related Documentation

IOUSBEndpointDescriptor

