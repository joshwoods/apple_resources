

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Options
-  setClientRequestHandler(\_:handler:) 

Instance Method

# setClientRequestHandler(\_:handler:)

Sets a handler to react to as a server to inbound WebSocket client handshakes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func setClientRequestHandler(
    _ queue: DispatchQueue,
    handler: @escaping ([String], [(name: String, value: String)]) -> NWProtocolWebSocket.Response
)
```

## See Also

### Handling Server Handshakes

struct Response

A WebSocket handshake reponse sent from a server to a client.

