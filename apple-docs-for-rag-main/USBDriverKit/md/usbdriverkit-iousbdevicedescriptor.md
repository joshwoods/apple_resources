

- USBDriverKit
-  IOUSBDeviceDescriptor 

Structure

# IOUSBDeviceDescriptor

The structure for storing a USB device descriptor.

DriverKit 19.0+

``` source
struct IOUSBDeviceDescriptor;
```

## Overview

For information about this descriptor type, see section 9.6.1 of the USB 3.2 specification at http://www.usb.org.

## Topics

### Getting the Device Properties

bLength

The length of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

bcdUSB

The USB specification release number with which the device complies.

bDeviceClass

The class code indicating the behavior of this device.

bDeviceSubClass

The subclass code that further defines the behavior of this device.

bDeviceProtocol

The protocol that the device supports.

bMaxPacketSize0

The maximum packet size for endpoint `0`, specified as an exponent value.

idVendor

The ID of the device’s manufacturer.

idProduct

The product ID assigned by the manufacturer.

bcdDevice

The release number of the device, specified as a binary-coded decimal number.

iManufacturer

The index of the string descriptor that describes the manufacturer.

iProduct

The index of the string descriptor that describes the product.

iSerialNumber

The index of the string descriptor that describes the device’s serial number.

bNumConfigurations

The number of configurations that the device supports.

## See Also

### Device Descriptors

IOUSBDeviceQualifierDescriptor

The structure for storing a USB device qualifier descriptor.

Apple’s Vendor ID

Apple’s vendor ID, assigned by the USB-IF.

