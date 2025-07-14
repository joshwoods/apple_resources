

- Network
- NWConnectionGroup
- NWConnectionGroup.Message
-  remoteEndpoint 

Instance Property

# remoteEndpoint

The endpoint that originates the message you receive.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var remoteEndpoint: NWEndpoint? { get }
```

## See Also

### Inspecting Received Messages

var localEndpoint: NWEndpoint?

The local address and port you use to receive the message.

var path: NWPath?

The network path on which you receive the message.

