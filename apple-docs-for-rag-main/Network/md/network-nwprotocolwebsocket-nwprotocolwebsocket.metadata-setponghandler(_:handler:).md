

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Metadata
-  setPongHandler(\_:handler:) 

Instance Method

# setPongHandler(\_:handler:)

Sets a handler on a Ping message to be invoked when the corresponding Pong message is received.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func setPongHandler(
    _ queue: DispatchQueue,
    handler: @escaping (NWError?) -> Void
)
```

## See Also

### Sending Messages

init(opcode: NWProtocolWebSocket.Opcode)

Initializes a WebSocket message with a specific type code.

enum Opcode

Types of messages that you send and receive on a WebSocket connection.

var closeCode: NWProtocolWebSocket.CloseCode

The close code on a WebSocket message.

enum CloseCode

Types of codes used upon closing a WebSocket connection.

