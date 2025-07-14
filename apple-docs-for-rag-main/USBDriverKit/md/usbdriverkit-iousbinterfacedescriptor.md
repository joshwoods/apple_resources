

- USBDriverKit
-  IOUSBInterfaceDescriptor 

Structure

# IOUSBInterfaceDescriptor

A descriptor for a specific interface of a USB device.

DriverKit 19.0+

``` source
struct IOUSBInterfaceDescriptor;
```

## Overview

An IOUSBInterfaceDescriptor object contains information about one of the device’s supported interfaces. A device’s configuration provides one or more interfaces, each with zero or more endpoints that define how to configure the pipes for that device.

For more information about this descriptor type, see section 9.6.5 of the USB 2.0 specification at http://www.usb.org.

## Topics

### Accessing the Descriptor Properties

bLength

The size of this descriptor in bytes.

bDescriptorType

A constant value indicating an interface descriptor.

bInterfaceNumber

The zero-based index of this interface in the current configuration.

bAlternateSetting

The alternative setting for the interface.

bNumEndpoints

The number of endpoints that this interface uses.

bInterfaceClass

The class code indicating the behavior of this interface.

bInterfaceSubClass

The subclass code that further defines the behavior of this interface.

bInterfaceProtocol

The protocol that this interface supports.

iInterface

The index of a string descriptor that describes this interface.

## See Also

### Interface Descriptors

IOUSBInterfaceAssociationDescriptor

The USB Interface Association Descriptor.

