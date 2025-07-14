

- USBDriverKit
-  IOUSBGetNextEndpointDescriptor 

Function

# IOUSBGetNextEndpointDescriptor

Finds the next endpoint descriptor associated with an interface descriptor.

DriverKit 19.0+

``` source
const IOUSBEndpointDescriptor * IOUSBGetNextEndpointDescriptor(const IOUSBConfigurationDescriptor * configurationDescriptor, const IOUSBInterfaceDescriptor * interfaceDescriptor, const IOUSBDescriptorHeader * currentDescriptor);
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`interfaceDescriptor`  

An interface descriptor within the bounds of the configuration descriptor.

`currentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor, or `NULL`.

## Return Value

An endpoint descriptor pointer, or `NULL` if no matching descriptor can be found.

## Discussion

This method uses `getNextAssociatedDescriptorWithType` to fetch the next endpoint descriptor associated with a specific interface descriptor.

## See Also

### Endpoint Descriptors

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

IOUSBGetEndpointNumber

Extracts the number of an endpoint from an endpoint descriptor.

IOUSBGetEndpointType

Extracts the type of an endpoint from an endpoint descriptor.

