

- USBDriverKit
-  IOUSBStandardEndpointDescriptors 

Structure

# IOUSBStandardEndpointDescriptors

Encapsulates the descriptors for a single endpoint.

DriverKit 19.0+

``` source
struct IOUSBStandardEndpointDescriptors;
```

## Discussion

Use this structure to intialize and adjust pipes in the system. You must initialize the bcdUSB member to the USB revision supported by the device. Acceptable values are `0x0110`, `0x0200`, `0x0300`, `0x0310`.

Initialize the descriptor field with a pointer to a valid endpoint descriptor. The ssCompanionDescriptor and sspCompanionDescriptor fields may be required for USB versions `0x0300` and greater, depending on device operating speed and values set in the descriptors.

For more information on when you must use these descriptors, see section 9.5 of the USB 3.1 specification.

## Topics

### Getting the Descriptors

bcdUSB

The USB version supported by the device, specified as a binary-coded decimal value.

descriptor

A valid endpoint descriptor.

ssCompanionDescriptor

The companion descriptor for super-speed devices.

sspCompanionDescriptor

The companion descriptor for super-speed plus devices.

## See Also

### Getting the Endpoint Descriptors

GetDescriptors

Retrieves the endpoint descriptors associated with this pipe.

IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

