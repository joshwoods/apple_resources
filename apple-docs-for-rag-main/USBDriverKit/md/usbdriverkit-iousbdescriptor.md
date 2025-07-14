

- USBDriverKit
-  IOUSBDescriptor 

Type Alias

# IOUSBDescriptor

The base descriptor type.

DriverKit 19.0+

``` source
typedef IOUSBDescriptorHeader IOUSBDescriptor;
```

## Discussion

Use this type to represent generic descriptor definitions. For more information about descriptors, see section 9.5 of the USB 2.0 specification at https://www.usb.org/.

## See Also

### Descriptor Fundamentals

IOUSBDescriptorHeader

The base descriptor header.

tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

