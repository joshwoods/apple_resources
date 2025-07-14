

- USBDriverKit
-  IOUSBGetEndpointNumber 

Function

# IOUSBGetEndpointNumber

Extracts the number of an endpoint from an endpoint descriptor.

DriverKit 19.0+

``` source
uint8_t IOUSBGetEndpointNumber(const IOUSBEndpointDescriptor * descriptor);
```

## Parameters 

`descriptor`  

The descriptor to parse.

## Return Value

An unsigned integer that represents an endpoint number.

## Discussion

This method parses an endpoint descriptor to determine its number, excluding direction.

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

IOUSBGetEndpointMult

Extracts the mult count from endpoint descriptors.

IOUSBGetEndpointType

Extracts the type of an endpoint from an endpoint descriptor.

