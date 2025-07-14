

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Response
-  init(status:subprotocol:additionalHeaders:) 

Initializer

# init(status:subprotocol:additionalHeaders:)

Initializes a WebSocket server response with a status, selected subprotocol, and additional HTTP headers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    status: NWProtocolWebSocket.Response.Status,
    subprotocol: String?,
    additionalHeaders: [(name: String, value: String)]? = nil
)
```

## See Also

### Sending Handshake Responses

enum Status

Status values that are sent with a WebSocket server response.

let status: NWProtocolWebSocket.Response.Status

The status of a WebSocket server response.

let subprotocol: String?

The selected subprotocol in a WebSocket server response.

let additionalHeaders: [(name: String, value: String)]?

Any additional HTTP headers in a WebSocket server response.

