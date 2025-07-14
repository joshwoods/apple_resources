

- USBDriverKit
-  tIOUSBDeviceRequestRecipientValue 

Enumeration

# tIOUSBDeviceRequestRecipientValue

Constants indicating the type of object that receives the results of a request.

DriverKit 19.0+

``` source
enum tIOUSBDeviceRequestRecipientValue : unsigned int;
```

## Topics

### Getting the Request Recipient

kIOUSBDeviceRequestRecipientValueDevice

The recipient is a device object.

kIOUSBDeviceRequestRecipientValueInterface

The recipient is an interface object.

kIOUSBDeviceRequestRecipientValueEndpoint

The recipient is an endpoint.

kIOUSBDeviceRequestRecipientValueOther

The recipient is another type of entity.

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

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

