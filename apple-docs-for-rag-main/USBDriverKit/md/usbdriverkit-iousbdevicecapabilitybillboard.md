

- USBDriverKit
-  IOUSBDeviceCapabilityBillboard 

Structure

# IOUSBDeviceCapabilityBillboard

The structure for the billboard device capability.

DriverKit 19.0+

``` source
struct IOUSBDeviceCapabilityBillboard;
```

## Overview

For more information about this descriptor type, see section 6.2 of the USB 3.1 specification at http://www.usb.org.

## Topics

### Accessing the Descriptor Properties

bLength

bDescriptorType

bDevCapabilityType

iAdditionalInfoURL

bNumberOfAlternateModes

bPreferredAlternateMode

vCONNPower

bmConfigured

bcdVersion

bAdditionalFailureInfo

bReserved

pAltConfigurations

## See Also

### Capability Descriptors

IOUSBBOSDescriptor

The structure for storing a binary object store (BOS) descriptor.

IOUSBDeviceCapabilityDescriptorHeader

The device capability descriptor header.

IOUSBDeviceCapabilityBillboardAltConfig

The structure for the billboard alternative configuration device capability.

IOUSBDeviceCapabilityBillboardAltConfigCompatibility

The structure for the billboard alternative configuration compatibility device capability.

IOUSBDeviceCapabilityBillboardAltMode

The structure for the billboard alternative mode device capability.

IOUSBDeviceCapabilityContainerID

The structure for the container ID device capability.

IOUSBDeviceCapabilitySuperSpeedUSB

The structure for the super-speed USB device capability.

IOUSBDeviceCapabilitySuperSpeedPlusUSB

The structure for the super-speed plus USB device capability.

IOUSBDeviceCapabilityUSB2Extension

The structure for the USB 2 extension device capability.

IOUSBPlatformCapabilityDescriptor

The structure for the platform capability descriptor.

tIOUSBDeviceCapabilityType

Constants for the device capability types.

SuperSpeed Device Capabilities

Constants for configuring super-speed device capabilities.

SuperSpeedPlus Device Capabilities

Constants for configuring super-speed plus device capabilities.

