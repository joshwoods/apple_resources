

- USBDriverKit
- IOUSBHostInterface
-  CopyStringDescriptor 

Instance Method

# CopyStringDescriptor

Returns a descriptor from the device in the specified language.

DriverKit 19.0+

``` source
const IOUSBStringDescriptor * CopyStringDescriptor(uint8_t index, uint16_t languageID);
```

## Parameters 

`index`  

The descriptor’s index value.

`languageID`  

The descriptor’s language ID. You can get the current list of valid language IDs at https://www.usb.org/.

## Return Value

A pointer to the descriptor, or `NULL` if the descriptor isn’t found. It’s your responsibility to free the returned descriptor.

## Discussion

This method uses a `GET_DESCRIPTOR` control request (USB 2.0, section 9.4.3) to fetch the string descriptor from the device. The method puts the `index` value in the low byte of the `wValue` field, and puts the `languageID` value in the `wIndex` field of the request structure.

## See Also

### Getting Interface-Related Descriptors

CopyConfigurationDescriptor

Retrieves the parent configuration descriptor for this interface.

GetInterfaceDescriptor

Returns the version of the interface descriptor that is associated with the specified configuration.

CopyStringDescriptor

Returns a string descriptor from the device.

