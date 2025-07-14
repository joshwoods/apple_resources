

- USBDriverKit
-  IOUSBGetEndpointMult 

Function

# IOUSBGetEndpointMult

Extracts the mult count from endpoint descriptors.

DriverKit 19.0+

``` source
uint8_t IOUSBGetEndpointMult(uint32_t usbDeviceSpeed, const IOUSBEndpointDescriptor * descriptor, const IOUSBSuperSpeedEndpointCompanionDescriptor * companionDescriptor, const IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor * sspCompanionDescriptor);
```

## Parameters 

`usbDeviceSpeed`  

The operational speed of the device.

`descriptor`  

The endpoint descriptor to parse.

`companionDescriptor`  

The companion descriptor to parse, or `NULL`.

`sspCompanionDescriptor`  

The SSP companion descriptor to parse, or `NULL`.

## Return Value

The mult count.

## Discussion

This method parses endpoint descriptors to determine mult.

## See Also

### Endpoint Descriptors

IOUSBGetNextEndpointDescriptor

Finds the next endpoint descriptor associated with an interface descriptor.

IOUSBGetEndpointAddress

Extracts the direction and number of an endpoint from an endpoint descriptor.

IOUSBGetEndpointBurstSize

Extracts the burst size from endpoint descriptors.

IOUSBGetEndpointDirection

Extracts the direction of an endpoint from an endpoint descriptor.

IOUSBGetEndpointIntervalEncodedMicroframes

Extracts the interval of an endpoint descriptor.

IOUSBGetEndpointIntervalFrames

Extracts the interval of an endpoint descriptor.

IOUSBGetEndpointIntervalMicroframes

Extracts the interval of an endpoint descriptor.

IOUSBGetEndpointMaxPacketSize

Extracts the maximum packet size from an endpoint descriptor.

IOUSBGetEndpointMaxStreams

Extracts the number of streams an endpoint supports.

IOUSBGetEndpointMaxStreamsEncoded

Extracts the number of streams an endpoint supports.

IOUSBGetEndpointNumber

Extracts the number of an endpoint from an endpoint descriptor.

IOUSBGetEndpointType

Extracts the type of an endpoint from an endpoint descriptor.

