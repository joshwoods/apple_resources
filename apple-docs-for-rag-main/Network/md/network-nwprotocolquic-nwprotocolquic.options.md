

- Network
- NWProtocolQUIC
-  NWProtocolQUIC.Options 

Class

# NWProtocolQUIC.Options

A container of options that configure the use of QUIC on a connection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class Options
```

## Topics

### Customizing Connection Options

convenience init(alpn: [String])

Initializes a default set of QUIC options along with a set of supported Application-Layer Protocol Negotiation values.

init()

Initializes a default set of QUIC options, without specifying a set of supported Application-Layer Protocol Negotiation values.

var alpn: [String]

A set of supported Application-Layer Protocol Negotiation values.

var idleTimeout: Int

The idle timeout for the QUIC connection, in milliseconds.

var initialMaxData: Int

A QUIC connection’s initial maximum data transport parameter.

var initialMaxStreamDataBidirectionalLocal: Int

A QUIC connection’s initial maximum stream data limit for locally-initiated bidirectional streams.

var initialMaxStreamDataBidirectionalRemote: Int

A QUIC connection’s initial maximum stream data limit for remote-initiated bidirectional streams.

var initialMaxStreamDataUnidirectional: Int

A QUIC connection’s initial maximum stream data limit for unidirectional streams.

var initialMaxStreamsBidirectional: Int

A QUIC connection’s initial maximum number of bidirectional streams.

var initialMaxStreamsUnidirectional: Int

A QUIC connection’s initial maximum number of unidirectional streams.

var maxDatagramFrameSize: Int

A QUIC connection’s maximum DATAGRAM frame size.

var maxUDPPayloadSize: Int

The maximum length of a QUIC packet that can be received on a connection, in bytes.

var securityProtocolOptions: sec_protocol_options_t

The handshake security options QUIC uses.

### Customizing Stream Options

var direction: NWProtocolQUIC.Options.Direction

The direction of the QUIC stream.

enum Direction

A directionality of a QUIC stream.

var isDatagram: Bool

A Boolean that indicates that this is a QUIC datagram flow, not a stream of bytes.

## Relationships

### Inherits From

- NWProtocolOptions

### Conforms To

- Sendable

## See Also

### Creating QUIC Connections

static let definition: NWProtocolDefinition

The system definition of the QUIC transport protocol.

