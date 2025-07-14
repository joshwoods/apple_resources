

- Network
- NWProtocolWebSocket
-  NWProtocolWebSocket.Opcode 

Enumeration

# NWProtocolWebSocket.Opcode

Types of messages that you send and receive on a WebSocket connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Opcode
```

## Topics

### Data Types

case binary

A binary data message.

case text

A text data message.

case cont

A continuation message.

### Control Types

case ping

A Ping message, which requests a Pong from the peer.

case pong

A Pong message in response to a Ping from the peer.

case close

A message indicating a close of the connection.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Sending Messages

init(opcode: NWProtocolWebSocket.Opcode)

Initializes a WebSocket message with a specific type code.

func setPongHandler(DispatchQueue, handler: (NWError?) -> Void)

Sets a handler on a Ping message to be invoked when the corresponding Pong message is received.

var closeCode: NWProtocolWebSocket.CloseCode

The close code on a WebSocket message.

enum CloseCode

Types of codes used upon closing a WebSocket connection.

