

- Network
- NWProtocolQUIC
- NWProtocolQUIC.Options
-  initialMaxData 

Instance Property

# initialMaxData

A QUIC connection’s initial maximum data transport parameter.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var initialMaxData: Int { get set }
```

## Discussion

This property determines the value of the `initial_max_data` transport parameter.

## See Also

### Customizing Connection Options

convenience init(alpn: [String])

Initializes a default set of QUIC options along with a set of supported Application-Layer Protocol Negotiation values.

init()

Initializes a default set of QUIC options, without specifying a set of supported Application-Layer Protocol Negotiation values.

var alpn: [String]

A set of supported Application-Layer Protocol Negotiation values.

var idleTimeout: Int

The idle timeout for the QUIC connection, in milliseconds.

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

