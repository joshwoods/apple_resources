

- Network
- NWProtocolQUIC
-  NWProtocolQUIC.Metadata 

Class

# NWProtocolQUIC.Metadata

A handle you can use to inspect a connection’s QUIC state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class Metadata
```

## Topics

### Inspecting Connection State

var negotiatedALPN: String?

The Application-Layer Protocol Negotiation value used when establishing the connection.

var localMaxStreamsBidirectional: Int

The maximum number of bidirectional streams that the peer can create on a QUIC connection.

var localMaxStreamsUnidirectional: Int

The maximum number of unidirectional streams that the peer can create on a QUIC connection.

var remoteMaxStreamsBidirectional: Int

The maximum number of bidirectional streams advertised by peer that the connection is allowed to create.

var remoteMaxStreamsUnidirectional: Int

The maximum number of unidirectional streams advertised by peer that the connection is allowed to create.

var remoteIdleTimeout: Int

The idle timeout value from the peer’s transport parameters, in milliseconds.

var securityProtocolMetadata: sec_protocol_metadata_t

The result of the QUIC handshake.

### Inspecting Stream State

var streamIdentifier: UInt64

The QUIC stream identifier.

var usableDatagramFrameSize: Int

The maximum usable size of a datagram frame on a QUIC datagram flow.

### Handling Errors

var applicationError: NWProtocolQUIC.ApplicationError

The QUIC application error code to send for the connection, or received from the peer.

struct ApplicationError

A QUIC application error code.

var streamApplicationErrorCode: UInt64

The QUIC application error code to send for the stream, or received from the peer.

### Configuring Keepalives

var keepAlive: NWProtocolQUIC.Metadata.KeepAliveBehavior

The QUIC connection keepalive behavior.

enum KeepAliveBehavior

A QUIC connection keepalive behavior.

## Relationships

### Inherits From

- NWProtocolMetadata

### Conforms To

- Sendable

