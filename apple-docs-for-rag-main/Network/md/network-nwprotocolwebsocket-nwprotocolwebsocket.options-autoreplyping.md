

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Options
-  autoReplyPing 

Instance Property

# autoReplyPing

A Boolean indicating whether the connection automatically replies to Ping messages instead of delivering them to you.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var autoReplyPing: Bool { get set }
```

## See Also

### Configuring WebSocket Options

init(NWProtocolWebSocket.Version)

Initializes a default set of WebSocket connection options.

enum Version

Supported versions of the WebSocket protocol.

var maximumMessageSize: Int

The maximum allowed message size, in bytes, to be received by the WebSocket connection.

