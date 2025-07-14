

- USBDriverKit
-  tIOUSBDeviceRequestTypeValue 

Enumeration

# tIOUSBDeviceRequestTypeValue

Constants indicating the type of request to make from a device.

DriverKit 19.0+

``` source
enum tIOUSBDeviceRequestTypeValue : unsigned int;
```

## Topics

### Getting the Request Type

kIOUSBDeviceRequestTypeValueStandard

A standard device request.

kIOUSBDeviceRequestTypeValueClass

A class-specific device request.

kIOUSBDeviceRequestTypeValueVendor

A vendor-specific device request.

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

tIOUSBDeviceRequestRecipientValue

Constants indicating the type of object that receives the results of a request.

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

