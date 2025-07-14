

- Network
- NWProtocolWebSocket
-  NWProtocolWebSocket.Version 

Enumeration

# NWProtocolWebSocket.Version

Supported versions of the WebSocket protocol.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Version
```

## Topics

### Versions

case version13

Version 13 of the WebSocket protocol.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Configuring WebSocket Options

init(NWProtocolWebSocket.Version)

Initializes a default set of WebSocket connection options.

var autoReplyPing: Bool

A Boolean indicating whether the connection automatically replies to Ping messages instead of delivering them to you.

var maximumMessageSize: Int

The maximum allowed message size, in bytes, to be received by the WebSocket connection.

