

- Network
- NWConnectionGroup
-  send(content:to:message:completion:) 

Instance Method

# send(content:to:message:completion:)

Sends data to the entire group, or to a specific member of the group.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@preconcurrency
final func send(
    content: Data?,
    to: NWEndpoint? = nil,
    message: NWConnectionGroup.Message = .default,
    completion: @escaping (NWError?) -> Void
)
```

## Parameters 

`content`  

The data to send.

`to`  

An optional endpoint that specifies a member of the group that receives the data. If the endpoint is `nil`, the data will be sent to the entire group.

`message`  

The metadata that defines how the message is sent.

`completion`  

A completion that notifies you when the connection group has processed and sent the data.

## See Also

### Sending and Receiving Group Messages

func setReceiveHandler(maximumMessageSize: Int, rejectOversizedMessages: Bool, handler: ((NWConnectionGroup.Message, Data?, Bool) -> Void)?)

Sets a handler that receives inbound messages from members of the group.

class Message

An object that represents a message that you send or receive within a group, and that contains protocol metadata and send properties.

