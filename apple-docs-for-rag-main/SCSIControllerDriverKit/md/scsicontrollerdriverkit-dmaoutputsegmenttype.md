

- SCSIControllerDriverKit
-  DMAOutputSegmentType 

Enumeration

# DMAOutputSegmentType

The size and endianness that the system uses for direct memory access (DMA).

DriverKit

``` source
typedef enum DMAOutputSegmentType : uint16_t { ... } DMAOutputSegmentType;
```

## Topics

### Segment Types

kDMAOutputSegmentBig32

A constant representing big-endian 32-bit DMA segments.

kDMAOutputSegmentBig64

A constant representing big-endian 64-bit DMA segments.

kDMAOutputSegmentHost32

A constant representing 32-bit DMA segments with host-native endianness.

kDMAOutputSegmentHost64

A constant representing 64-bit DMA segments with host-native endianness.

kDMAOutputSegmentLittle32

A constant representing little-endian 32-bit DMA segments.

kDMAOutputSegmentLittle64

A constant representing little-endian 64-bit DMA segments.

## See Also

### Managing Direct Memory Access

UserGetDMASpecification

Gets the controller-specific direct memory access (DMA) specification in response to a call from the framework.

