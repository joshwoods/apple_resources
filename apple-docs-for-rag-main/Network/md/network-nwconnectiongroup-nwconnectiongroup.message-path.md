

- Network
- NWConnectionGroup
- NWConnectionGroup.Message
-  path 

Instance Property

# path

The network path on which you receive the message.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var path: NWPath? { get }
```

## See Also

### Inspecting Received Messages

var remoteEndpoint: NWEndpoint?

The endpoint that originates the message you receive.

var localEndpoint: NWEndpoint?

The local address and port you use to receive the message.

