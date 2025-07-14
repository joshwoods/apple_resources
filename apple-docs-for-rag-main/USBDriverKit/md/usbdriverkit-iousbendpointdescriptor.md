

- USBDriverKit
-  IOUSBEndpointDescriptor 

Structure

# IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

DriverKit 19.0+

``` source
struct IOUSBEndpointDescriptor;
```

## Overview

For more information about this descriptor type, see section 9.6.6 of the USB 2.0 specification at http://www.usb.org.

## Topics

### Accessing the Descriptor Properties

bLength

The length of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

bEndpointAddress

The address of the endpoint.

bmAttributes

The attributes of the endpoint.

wMaxPacketSize

The maximum packet size that the endpoint supports.

bInterval

The interval to use when polling the endpoint for data transfers, specified in frames or microframes depending on the device’s speed.

## See Also

### Endpoint Descriptors

IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB Endpoint Companion.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus Isochronous USB Endpoint Companion.

tIOUSBEndpointType

Constants describing the types of endpoints.

Endpoint Attributes

Constants for endpoint attributes.

SuperSpeed USB Endpoint Descriptor Options

Constants for super-speed endpoint attributes.

tIOUSBEndpointDirection

The direction of data transfers on an endpoint.

tIOUSBEndpointSynchronizationType

Constants for the endpoint synchronization types.

tIOUSBEndpointUsageType

Constants for the endpoint usage types.

tIOUSBLanguageID

Constants for the USB language identifiers.

