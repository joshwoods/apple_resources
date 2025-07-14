

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBStandardEndpointDescriptors 

# IOUSBStandardEndpointDescriptors

A container for descriptors for a single endpoint.

macOS 10.15+

``` source
struct IOUSBStandardEndpointDescriptors {
    ...
};
```

## Discussion

Use this structure to intialize and adjust pipes in the system. You must initialize the `bcdUSB` descriptor to the USB version that the device supports. Acceptable values are `0x0110`, `0x0200`, `0x0300`, `0x0310`.

Initialize the descriptor field with a pointer to a valid endpoint descriptor. USB versions `0x0300` and greater may require the ssCompanionDescriptor and sspCompanionDescriptor fields, depending on device operating speed and values set in the descriptors.

For more information on when you must use these descriptors, see USB 3.2, 9.5.

## Topics

### Getting the Properties

bcdUSB

A binary-coded decimal value that indicates the USB version that the device supports.

descriptor

A valid endpoint descriptor.

ssCompanionDescriptor

The companion descriptor for SuperSpeed devices.

sspCompanionDescriptor

The companion descriptor for SuperSpeedPlus devices.

## See Also

### Endpoint Descriptors

IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

IOUSBEndpointDescriptorPtr

A pointer to the endpoint descriptor.

IOUSBEndpointProperties

A structure that holds USB endpoint properties.

IOUSBEndpointPropertiesPtr

A pointer to an endpoint properties object.

IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

