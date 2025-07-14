

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Metadata
-  additionalServerHeaders 

Instance Property

# additionalServerHeaders

Additional HTTP headers sent by the server during the WebSocket handshake.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var additionalServerHeaders: [(String, String)]? { get }
```

## See Also

### Inspecting Handshake Results

var selectedSubprotocol: String?

The subprotocol selected by the server during the WebSocket handshake.

