

- Network
- NWProtocolWebSocket
-  NWProtocolWebSocket.Options 

Class

# NWProtocolWebSocket.Options

A container of options for configuring how WebSocket is used on a connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class Options
```

## Topics

### Configuring WebSocket Options

init(NWProtocolWebSocket.Version)

Initializes a default set of WebSocket connection options.

enum Version

Supported versions of the WebSocket protocol.

var autoReplyPing: Bool

A Boolean indicating whether the connection automatically replies to Ping messages instead of delivering them to you.

var maximumMessageSize: Int

The maximum allowed message size, in bytes, to be received by the WebSocket connection.

### Configuring Client Handshakes

func setAdditionalHeaders([(name: String, value: String)])

Sets additional HTTP header fields to be sent by the client during the WebSocket handshake.

func setSubprotocols([String])

Adds to the list of supported application protocols that will be presented to a WebSocket server during connection establishment.

var skipHandshake: Bool

A Boolean indicating whether the WebSocket protocol skips its handshake and begins framing data once the underlying connection is established.

### Handling Server Handshakes

func setClientRequestHandler(DispatchQueue, handler: ([String], [(name: String, value: String)]) -> NWProtocolWebSocket.Response)

Sets a handler to react to as a server to inbound WebSocket client handshakes.

struct Response

A WebSocket handshake reponse sent from a server to a client.

## Relationships

### Inherits From

- NWProtocolOptions

### Conforms To

- Sendable

## See Also

### Creating WebSocket Connections

static let definition: NWProtocolDefinition

The system definition of the WebSocket protocol.

