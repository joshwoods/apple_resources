

- USBDriverKit
-  IOUSBSuperSpeedHubDescriptor 

Structure

# IOUSBSuperSpeedHubDescriptor

A structure that defines the descriptor for a Super Speed USB hub.

DriverKit 19.0+

``` source
struct IOUSBSuperSpeedHubDescriptor;
```

## Overview

For more information about this descriptor type, see section 10.13.2.1 of the USB 3.0 specification at http://www.usb.org.

## Topics

### Accessing the Descriptor Properties

bLength

bDescriptorType

bNumberPorts

wHubCharacteristics

bPowerOnToPowerGood

bHubControllerCurrent

bHubDecodeLatency

wHubDelay

deviceRemovable

## See Also

### USB Descriptors

IOUSB20HubDescriptor

A structure that defines the descriptor for a USB hub.

SuperSpeed Hub Characteristics

Constants for specifying super-speed hub characteristics.

UASPipeDescriptor

A structure that defines the Mass Storage Specific UAS pipe usage descriptor.

