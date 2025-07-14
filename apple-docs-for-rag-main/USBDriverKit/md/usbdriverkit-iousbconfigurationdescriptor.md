

- USBDriverKit
-  IOUSBConfigurationDescriptor 

Structure

# IOUSBConfigurationDescriptor

The structure for storing a USB configuration descriptor.

DriverKit 19.0+

``` source
struct IOUSBConfigurationDescriptor;
```

## Overview

This descriptor contains information about a specific configuration of a device, including the interfaces that configuration provides. This structure has a variable length, so it defines only the known fields. Use the `wTotalLength` field to read the entire descriptor.

For more information about this descriptor type, see section 9.6.3 of the USB 2.0 specification at http://www.usb.org.

## Topics

### Getting the Descriptor Properties

bLength

The size of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

wTotalLength

The total length of the descriptor, including the length of all related interface, endpoint, and vendor-specific descriptors.

bNumInterfaces

The number of interfaces this configuration supports.

bConfigurationValue

The value to use when selecting this configuration.

iConfiguration

The index of the string descriptor that describes this configuration.

bmAttributes

A bitmask indicating the configuration’s characteristics.

MaxPower

The maximum power consumption of the USB device expressed in 2mA units.

## See Also

### Configuration Descriptors

IOUSBConfigurationDescHeader

The header of a configuration descriptor.

Power Configuration Settings

Constants for configuring the power settings.

