

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Options
-  skipHandshake 

Instance Property

# skipHandshake

A Boolean indicating whether the WebSocket protocol skips its handshake and begins framing data once the underlying connection is established.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var skipHandshake: Bool { get set }
```

## Discussion

This option should not be set when communicating with a generic WebSocket server or client. This option allows a custom handshake (or no handshake) to be implemented below the WebSocket layer when both client and server are coordinated.

## See Also

### Configuring Client Handshakes

func setAdditionalHeaders([(name: String, value: String)])

Sets additional HTTP header fields to be sent by the client during the WebSocket handshake.

func setSubprotocols([String])

Adds to the list of supported application protocols that will be presented to a WebSocket server during connection establishment.

