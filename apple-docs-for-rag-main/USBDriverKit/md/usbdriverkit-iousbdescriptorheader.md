

- USBDriverKit
-  IOUSBDescriptorHeader 

Structure

# IOUSBDescriptorHeader

The base descriptor header.

DriverKit 19.0+

``` source
struct IOUSBDescriptorHeader;
```

## Overview

For more information about descriptors, see section 9.5 of the USB 2.0 specification at https://www.usb.org/.

## Topics

### Getting the Descriptor Properties

bLength

The number of bytes in the descriptor.

bDescriptorType

The type of the descriptor.

## See Also

### Descriptor Fundamentals

IOUSBDescriptor

The base descriptor type.

tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

