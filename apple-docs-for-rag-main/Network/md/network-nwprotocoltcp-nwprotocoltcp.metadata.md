

- Network
- NWProtocolTCP
-  NWProtocolTCP.Metadata 

Class

# NWProtocolTCP.Metadata

A handle you can use to inspect a connection’s TCP state.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class Metadata
```

## Topics

### Inspecting TCP State

var availableSendBuffer: UInt32

The number of available bytes in the TCP send buffer.

var availableReceiveBuffer: UInt32

The number of available bytes in the TCP receive buffer.

## Relationships

### Inherits From

- NWProtocolMetadata

### Conforms To

- Sendable

