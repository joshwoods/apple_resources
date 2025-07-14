

- Network
-  NWProtocolWebSocket 

Class

# NWProtocolWebSocket

A network protocol for connections that use WebSocket.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NWProtocolWebSocket
```

## Topics

### Creating WebSocket Connections

class Options

A container of options for configuring how WebSocket is used on a connection.

static let definition: NWProtocolDefinition

The system definition of the WebSocket protocol.

### Handling WebSocket Messages

class Metadata

A WebSocket message you configure when sending and receiving packets.

### Structures

struct Response

A WebSocket handshake reponse sent from a server to a client.

### Enumerations

enum CloseCode

Types of codes used upon closing a WebSocket connection.

enum Opcode

Types of messages that you send and receive on a WebSocket connection.

enum Version

Supported versions of the WebSocket protocol.

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

class NWProtocolQUIC

A network protocol for connections that use the QUIC transport protocol.

class NWProtocolUDP

A network protocol for connections that use the User Datagram Protocol.

class NWProtocolIP

A network protocol for configuring the Internet Protocol on connections.

class NWProtocolFramer

A customizable network protocol for defining application message parsers.

