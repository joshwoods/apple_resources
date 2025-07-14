

- USBDriverKit
- IOUSBHostDevice
-  CopyStringDescriptor 

Instance Method

# CopyStringDescriptor

Returns a string descriptor from the device.

DriverKit 19.0+

``` source
const IOUSBStringDescriptor * CopyStringDescriptor(uint8_t index, uint16_t languageID);
```

## Parameters 

`index`  

The descriptor index value. This parameter corresponds to the low byte of `wValue` of the `SET_DESCRIPTOR` control request (USB 2.0, section 9.4.8).

`languageID`  

The descriptor language ID. This parameter corresponds to the `wIndex` value of the `SET_DESCRIPTOR` control request (USB 2.0, section 9.4.8).

## Return Value

A pointer to the descriptor, if found. It’s your responsibility to free the returned descriptor.

## Discussion

This method searches the descriptor cache for the specified descriptor. If the descriptor isn’t in the cache, the method retrieves it from the device using a `GET_DESCRIPTOR` control request (USB 2.0, section 9.4.3) and adds it to the cache. When making a `GET_DESCRIPTOR` control request, this method acquires the service’s workloop lock and may call commandSleep.

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

CopyDescriptor

Retrieves any type of descriptor from the cache or the device.

tIOUSBDeviceRequestTypeValue

Constants indicating the type of request to make from a device.

tIOUSBDeviceRequestRecipientValue

Constants indicating the type of object that receives the results of a request.

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

