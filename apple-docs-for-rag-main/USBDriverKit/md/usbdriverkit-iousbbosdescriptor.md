

- USBDriverKit
-  IOUSBBOSDescriptor 

Structure

# IOUSBBOSDescriptor

The structure for storing a binary object store (BOS) descriptor.

DriverKit 19.0+

``` source
struct IOUSBBOSDescriptor;
```

## Overview

For more information about this descriptor type, see section 9.6.2 of the USB 3.2 specification at http://www.usb.org.

## Topics

### Accessing the Descriptor Properties

bLength

The size of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

wTotalLength

The length, in bytes, of the descriptor and all of its subdescriptors.

bNumDeviceCaps

The number of separate device capability descriptors in the binary object store.

## See Also

### Capability Descriptors

IOUSBDeviceCapabilityDescriptorHeader

The device capability descriptor header.

IOUSBDeviceCapabilityBillboard

The structure for the billboard device capability.

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

