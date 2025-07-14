

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.Options
-  init(\_:) 

Initializer

# init(\_:)

Initializes a default set of WebSocket connection options.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ version: NWProtocolWebSocket.Version = .version13)
```

## See Also

### Configuring WebSocket Options

enum Version

Supported versions of the WebSocket protocol.

var autoReplyPing: Bool

A Boolean indicating whether the connection automatically replies to Ping messages instead of delivering them to you.

var maximumMessageSize: Int

The maximum allowed message size, in bytes, to be received by the WebSocket connection.

