

- USBDriverKit
- IOUSBHostDevice
-  CopyConfigurationDescriptor 

Instance Method

# CopyConfigurationDescriptor

Returns the currently selected configuration descriptor.

DriverKit 19.0+

``` source
const IOUSBConfigurationDescriptor * CopyConfigurationDescriptor(IOService * forClient);
```

## Parameters 

`forClient`  

The current service object. You may specify `NULL` for this parameter.

## Return Value

A pointer to the configuration descriptor if found, or `NULL` if the device isn’t configured. It’s your responsibility to free the returned descriptor.

## Discussion

This method searches the descriptor cache for the specified descriptor. If the descriptor isn’t in the cache, the method retrieves it from the device using a `GET_DESCRIPTOR` control request (USB 2.0, section 9.4.3) and adds it to the cache. When making a `GET_DESCRIPTOR` control request, this method acquires the service’s workloop lock and may call commandSleep.

## See Also

### Getting the Device Descriptors

CopyCapabilityDescriptors

Returns the device’s capability descriptors.

CopyConfigurationDescriptor

Returns the configuration descriptor with the specified index.

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

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

