

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Metadata
-  init(opcode:) 

Initializer

# init(opcode:)

Initializes a WebSocket message with a specific type code.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(opcode: NWProtocolWebSocket.Opcode)
```

## See Also

### Sending Messages

enum Opcode

Types of messages that you send and receive on a WebSocket connection.

func setPongHandler(DispatchQueue, handler: (NWError?) -> Void)

Sets a handler on a Ping message to be invoked when the corresponding Pong message is received.

var closeCode: NWProtocolWebSocket.CloseCode

The close code on a WebSocket message.

enum CloseCode

Types of codes used upon closing a WebSocket connection.

