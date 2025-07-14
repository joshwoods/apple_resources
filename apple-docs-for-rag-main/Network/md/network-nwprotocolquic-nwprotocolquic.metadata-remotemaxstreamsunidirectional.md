

- Network
- NWProtocolQUIC
- NWProtocolQUIC.Metadata
-  remoteMaxStreamsUnidirectional 

Instance Property

# remoteMaxStreamsUnidirectional

The maximum number of unidirectional streams advertised by peer that the connection is allowed to create.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var remoteMaxStreamsUnidirectional: Int { get }
```

## See Also

### Inspecting Connection State

var negotiatedALPN: String?

The Application-Layer Protocol Negotiation value used when establishing the connection.

var localMaxStreamsBidirectional: Int

The maximum number of bidirectional streams that the peer can create on a QUIC connection.

var localMaxStreamsUnidirectional: Int

The maximum number of unidirectional streams that the peer can create on a QUIC connection.

var remoteMaxStreamsBidirectional: Int

The maximum number of bidirectional streams advertised by peer that the connection is allowed to create.

var remoteIdleTimeout: Int

The idle timeout value from the peer’s transport parameters, in milliseconds.

var securityProtocolMetadata: sec_protocol_metadata_t

The result of the QUIC handshake.

