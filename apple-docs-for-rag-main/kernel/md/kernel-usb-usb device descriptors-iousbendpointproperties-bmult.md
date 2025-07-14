

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBEndpointProperties
-  bMult 

Instance Property

# bMult

The mult value for isochronous endpoints.

macOS 10.8+

``` source
UInt8 bMult;
```

## Discussion

For SuperSpeed isochronous endpoints, this is the mult value from the SuperSpeed endpoint companion descriptor. For high-speed isochronous and interrupt endpoints, this is bits 11 and 12 of the standard endpoint descriptor.

## See Also

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

wBytesPerInterval

The number of bytes per interval.

