

- USBDriverKit
-  IOUSBInterfaceAssociationDescriptor 

Structure

# IOUSBInterfaceAssociationDescriptor

The USB Interface Association Descriptor.

DriverKit 19.0+

``` source
struct IOUSBInterfaceAssociationDescriptor;
```

## Overview

This type defines the ECN to the USB 2.0 Spec. See the USB Specification at http://www.usb.org. USB 3.0 9.6.4: Interface Association.

## Topics

### Accessing the Descriptor Properties

bLength

bDescriptorType

bFirstInterface

bInterfaceCount

bFunctionClass

bFunctionSubClass

bFunctionProtocol

iFunction

## See Also

### Interface Descriptors

IOUSBInterfaceDescriptor

A descriptor for a specific interface of a USB device.

