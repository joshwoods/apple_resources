

- Network
- NWProtocolWebSocket
-  NWProtocolWebSocket.Metadata 

Class

# NWProtocolWebSocket.Metadata

A WebSocket message you configure when sending and receiving packets.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class Metadata
```

## Topics

### Sending Messages

init(opcode: NWProtocolWebSocket.Opcode)

Initializes a WebSocket message with a specific type code.

enum Opcode

Types of messages that you send and receive on a WebSocket connection.

func setPongHandler(DispatchQueue, handler: (NWError?) -> Void)

Sets a handler on a Ping message to be invoked when the corresponding Pong message is received.

var closeCode: NWProtocolWebSocket.CloseCode

The close code on a WebSocket message.

enum CloseCode

Types of codes used upon closing a WebSocket connection.

### Receiving Messages

let opcode: NWProtocolWebSocket.Opcode

The type code of a WebSocket message.

var closeCode: NWProtocolWebSocket.CloseCode

The close code on a WebSocket message.

enum CloseCode

Types of codes used upon closing a WebSocket connection.

### Inspecting Handshake Results

var selectedSubprotocol: String?

The subprotocol selected by the server during the WebSocket handshake.

var additionalServerHeaders: [(String, String)]?

Additional HTTP headers sent by the server during the WebSocket handshake.

## Relationships

### Inherits From

- NWProtocolMetadata

### Conforms To

- Sendable

