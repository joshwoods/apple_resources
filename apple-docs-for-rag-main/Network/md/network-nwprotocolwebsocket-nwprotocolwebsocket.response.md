

- Network
- NWProtocolWebSocket
-  NWProtocolWebSocket.Response 

Structure

# NWProtocolWebSocket.Response

A WebSocket handshake reponse sent from a server to a client.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Response
```

## Topics

### Sending Handshake Responses

init(status: NWProtocolWebSocket.Response.Status, subprotocol: String?, additionalHeaders: [(name: String, value: String)]?)

Initializes a WebSocket server response with a status, selected subprotocol, and additional HTTP headers.

enum Status

Status values that are sent with a WebSocket server response.

let status: NWProtocolWebSocket.Response.Status

The status of a WebSocket server response.

let subprotocol: String?

The selected subprotocol in a WebSocket server response.

let additionalHeaders: [(name: String, value: String)]?

Any additional HTTP headers in a WebSocket server response.

## Relationships

### Conforms To

- Sendable

## See Also

### Handling Server Handshakes

func setClientRequestHandler(DispatchQueue, handler: ([String], [(name: String, value: String)]) -> NWProtocolWebSocket.Response)

Sets a handler to react to as a server to inbound WebSocket client handshakes.

