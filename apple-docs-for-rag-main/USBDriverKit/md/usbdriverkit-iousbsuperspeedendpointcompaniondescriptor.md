

- USBDriverKit
-  IOUSBSuperSpeedEndpointCompanionDescriptor 

Structure

# IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB Endpoint Companion.

DriverKit 19.0+

``` source
struct IOUSBSuperSpeedEndpointCompanionDescriptor;
```

## Overview

For more information about this descriptor type, see section 9.6.7 of the USB 3.1 specification at http://www.usb.org.

## Topics

### Accessing the Descriptor Properties

bLength

The length of this descriptor in bytes.

bDescriptorType

The type of the descriptor.

bMaxBurst

The maximum number of packets the endpoint can send or receive in one burst.

bmAttributes

The attributes associated with the endpoint.

wBytesPerInterval

The total number of bytes this endpoint transfers during each service interval.

## See Also

### Endpoint Descriptors

IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

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

