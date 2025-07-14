

- USBDriverKit
-  IOUSB20HubDescriptor 

Structure

# IOUSB20HubDescriptor

A structure that defines the descriptor for a USB hub.

DriverKit 19.0+

``` source
struct IOUSB20HubDescriptor;
```

## Overview

For more information about this descriptor type, see section 11.23.2.1 of the USB 2.0 specification at http://www.usb.org.

## Topics

### Accessing the Descriptor Properties

bLength

bDescriptorType

bNumberPorts

wHubCharacteristics

bPowerOnToPowerGood

bHubControllerCurrent

deviceRemovable

reserved

## See Also

### USB Descriptors

IOUSBSuperSpeedHubDescriptor

A structure that defines the descriptor for a Super Speed USB hub.

SuperSpeed Hub Characteristics

Constants for specifying super-speed hub characteristics.

UASPipeDescriptor

A structure that defines the Mass Storage Specific UAS pipe usage descriptor.

