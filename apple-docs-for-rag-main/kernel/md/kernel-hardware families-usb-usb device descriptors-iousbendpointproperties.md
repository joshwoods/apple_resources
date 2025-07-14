

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBEndpointProperties 

Type Alias

# IOUSBEndpointProperties

A structure that holds USB endpoint properties.

macOS 10.8+

``` source
typedef struct IOUSBEndpointProperties IOUSBEndpointProperties;
```

## Discussion

Use this structure with the IOUSBLib GetEndpointPropertiesV3 and GetPipePropertiesV3 API. Most of the fields come directly from the corresponding standard endpoint descriptor and SuperSpeed endpoint companion descriptor.

The API synthesizes `wBytesPerInterval` for high-speed high-bandwidth isochronous endpoints.

## Topics

### Getting the Properties

bVersion

The version of the structure.

bAlternateSetting

The alternative setting for obtaining endpoint and pipe properties.

bDirection

The direction of the endpoint.

bEndpointNumber

The number of the endpoint.

bTransferType

The transfer type of the endpoint.

bUsageType

The usage type of the endpoint.

bSyncType

The type for isochronous endpoints.

bInterval

The interval field from the standard endpoint descriptor.

wMaxPacketSize

The maximum packet size.

bMaxBurst

The maximum number of packets the endpoint can send or receive for SuperSpeed endpoints.

bMaxStreams

The maximum number of streams this endpoint supports for SuperSpeed bulk endpoints.

bMult

The mult value for isochronous endpoints.

wBytesPerInterval

The number of bytes per interval.

## See Also

### Endpoint Descriptors

IOUSBEndpointDescriptor

The structure for storing an endpoint descriptor.

IOUSBStandardEndpointDescriptors

A container for descriptors for a single endpoint.

IOUSBEndpointDescriptorPtr

A pointer to the endpoint descriptor.

IOUSBEndpointPropertiesPtr

A pointer to an endpoint properties object.

IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

### Related Documentation

