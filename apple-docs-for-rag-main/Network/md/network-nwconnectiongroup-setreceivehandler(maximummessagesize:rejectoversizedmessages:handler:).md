

- Network
- NWConnectionGroup
-  setReceiveHandler(maximumMessageSize:rejectOversizedMessages:handler:) 

Instance Method

# setReceiveHandler(maximumMessageSize:rejectOversizedMessages:handler:)

Sets a handler that receives inbound messages from members of the group.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@preconcurrency
final func setReceiveHandler(
    maximumMessageSize: Int = Int.max,
    rejectOversizedMessages: Bool = true,
    handler: ((NWConnectionGroup.Message, Data?, Bool) -> Void)?
)
```

## See Also

### Sending and Receiving Group Messages

func send(content: Data?, to: NWEndpoint?, message: NWConnectionGroup.Message, completion: (NWError?) -> Void)

Sends data to the entire group, or to a specific member of the group.

class Message

An object that represents a message that you send or receive within a group, and that contains protocol metadata and send properties.

