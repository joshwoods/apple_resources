

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Options
-  maximumMessageSize 

Instance Property

# maximumMessageSize

The maximum allowed message size, in bytes, to be received by the WebSocket connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var maximumMessageSize: Int { get set }
```

## See Also

### Configuring WebSocket Options

init(NWProtocolWebSocket.Version)

Initializes a default set of WebSocket connection options.

enum Version

Supported versions of the WebSocket protocol.

var autoReplyPing: Bool

A Boolean indicating whether the connection automatically replies to Ping messages instead of delivering them to you.

