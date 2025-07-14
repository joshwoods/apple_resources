

- USBDriverKit
-  tIOUSBEndpointDirection 

Enumeration

# tIOUSBEndpointDirection

The direction of data transfers on an endpoint.

DriverKit 19.0+

``` source
enum tIOUSBEndpointDirection : unsigned int;
```

## Topics

### Getting the Endpoint Direction

kIOUSBEndpointDirectionOut

Data flows from the driver out to the device.

kIOUSBEndpointDirectionIn

Data flows from the device into the driver.

kIOUSBEndpointDirectionUnknown

The transfer direction is unknown.

## See Also

### Endpoint Descriptors

IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

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

tIOUSBEndpointSynchronizationType

Constants for the endpoint synchronization types.

tIOUSBEndpointUsageType

Constants for the endpoint usage types.

tIOUSBLanguageID

Constants for the USB language identifiers.

