

- USBDriverKit
-  IOUSBGetEndpointIntervalEncodedMicroframes 

Function

# IOUSBGetEndpointIntervalEncodedMicroframes

Extracts the interval of an endpoint descriptor.

DriverKit 19.0+

``` source
uint32_t IOUSBGetEndpointIntervalEncodedMicroframes(uint32_t usbDeviceSpeed, const IOUSBEndpointDescriptor * descriptor);
```

## Parameters 

`usbDeviceSpeed`  

The operational speed of the device.

`descriptor`  

The endpoint descriptor to parse.

## Return Value

The encoded endpoint interval.

## Discussion

This method parses an endpoint descriptor and returns the service interval as `n` in `(2^(n-1))` microframes.

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

IOUSBGetEndpointNumber

Extracts the number of an endpoint from an endpoint descriptor.

IOUSBGetEndpointType

Extracts the type of an endpoint from an endpoint descriptor.

