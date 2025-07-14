

- Network
- NWProtocolQUIC
- NWProtocolQUIC.Options
-  NWProtocolQUIC.Options.Direction 

Enumeration

# NWProtocolQUIC.Options.Direction

A directionality of a QUIC stream.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Direction
```

## Topics

### Direction Values

case bidirectional

A bidirectional QUIC stream.

case unidirectional

A unidirectional QUIC stream.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Customizing Stream Options

var direction: NWProtocolQUIC.Options.Direction

The direction of the QUIC stream.

var isDatagram: Bool

A Boolean that indicates that this is a QUIC datagram flow, not a stream of bytes.

