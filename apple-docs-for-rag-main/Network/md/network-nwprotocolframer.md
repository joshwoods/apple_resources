

- Network
-  NWProtocolFramer 

Class

# NWProtocolFramer

A customizable network protocol for defining application message parsers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NWProtocolFramer
```

## Topics

### Implementing Framer Protocols

protocol NWProtocolFramerImplementation

A protocol to which your classes can conform in order to implement a custom framing protocol.

class Instance

An object that represents a single instance of your custom protocol running in a connection.

### Using Framers with Connections

class Definition

A custom protocol definition you use to associate messages with protocol options.

class Options

A container you use to add your custom protocol to a connection’s protocol stack.

class Message

A message for a custom protocol, in which you can store arbitrary key-value pairs.

### Enumerations

enum StartResult

Results that you send to indicate the disposition of your protocol after receiving the call to start.

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

class NWProtocolWebSocket

A network protocol for connections that use WebSocket.

