

- Network
- NWConnectionGroup
- NWConnectionGroup.Message
-  localEndpoint 

Instance Property

# localEndpoint

The local address and port you use to receive the message.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var localEndpoint: NWEndpoint? { get }
```

## See Also

### Inspecting Received Messages

var remoteEndpoint: NWEndpoint?

The endpoint that originates the message you receive.

var path: NWPath?

The network path on which you receive the message.

