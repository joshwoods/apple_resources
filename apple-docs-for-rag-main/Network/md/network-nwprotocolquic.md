

- Network
-  NWProtocolQUIC 

Class

# NWProtocolQUIC

A network protocol for connections that use the QUIC transport protocol.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class NWProtocolQUIC
```

## Topics

### Creating QUIC Connections

class Options

A container of options that configure the use of QUIC on a connection.

static let definition: NWProtocolDefinition

The system definition of the QUIC transport protocol.

### Inspecting QUIC State

class Metadata

A handle you can use to inspect a connection’s QUIC state.

### Structures

struct ApplicationError

A QUIC application error code.

## Relationships

### Inherits From

- NWProtocol

### Conforms To

- Sendable

## See Also

### Network Protocols

Building a custom peer-to-peer protocol

Use networking frameworks to create a custom protocol for playing a game across iOS, iPadOS, watchOS, and tvOS devices.

class NWProtocolTCP

A network protocol for connections that use the Transmission Control Protocol.

class NWProtocolTLS

A network protocol for connections that use Transport Layer Security.

class NWProtocolUDP

A network protocol for connections that use the User Datagram Protocol.

class NWProtocolIP

A network protocol for configuring the Internet Protocol on connections.

class NWProtocolWebSocket

A network protocol for connections that use WebSocket.

class NWProtocolFramer

A customizable network protocol for defining application message parsers.

