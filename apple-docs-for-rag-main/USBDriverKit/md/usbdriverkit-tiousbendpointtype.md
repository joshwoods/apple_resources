

- USBDriverKit
-  tIOUSBEndpointType 

Enumeration

# tIOUSBEndpointType

Constants describing the types of endpoints.

DriverKit 19.0+

``` source
enum tIOUSBEndpointType : unsigned int;
```

## Topics

### Getting the Endpoint Types

kIOUSBEndpointTypeControl

A control endpoint for the device.

kIOUSBEndpointTypeBulk

An endpoint you use for bulk transfers.

kIOUSBEndpointTypeInterrupt

An endpoint you use for interrupts.

kIOUSBEndpointTypeIsochronous

An endpoint you use for isochronous transfers.

## See Also

### Endpoint Descriptors

IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB Endpoint Companion.

IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus Isochronous USB Endpoint Companion.

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

