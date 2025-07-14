

- Network
-  NWProtocolTCP 

Class

# NWProtocolTCP

A network protocol for connections that use the Transmission Control Protocol.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class NWProtocolTCP
```

## Topics

### Creating TCP Connections

class Options

A container of options for configuring how TCP is used on a connection.

static let definition: NWProtocolDefinition

The system definition of the Transport Control Protocol.

### Inspecting TCP State

class Metadata

A handle you can use to inspect a connection’s TCP state.

## Relationships

### Inherits From

- NWProtocol

### Conforms To

- Sendable

## See Also

### Network Protocols

Building a custom peer-to-peer protocol

Use networking frameworks to create a custom protocol for playing a game across iOS, iPadOS, watchOS, and tvOS devices.

class NWProtocolTLS

A network protocol for connections that use Transport Layer Security.

class NWProtocolQUIC

A network protocol for connections that use the QUIC transport protocol.

class NWProtocolUDP

A network protocol for connections that use the User Datagram Protocol.

class NWProtocolIP

A network protocol for configuring the Internet Protocol on connections.

class NWProtocolWebSocket

A network protocol for connections that use WebSocket.

class NWProtocolFramer

A customizable network protocol for defining application message parsers.

