

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBEndpointProperties
-  bUsageType 

Instance Property

# bUsageType

The usage type of the endpoint.

macOS 10.8+

``` source
UInt8 bUsageType;
```

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

