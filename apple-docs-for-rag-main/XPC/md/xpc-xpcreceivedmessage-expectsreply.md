

- XPC
- XPCReceivedMessage
-  expectsReply 

Instance Property

# expectsReply

A Boolean value that indicates if the client that sent the message expects a reply.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
var expectsReply: Bool { get }
```

## See Also

### Replying to messages

func reply&lt;Message>(Message)

Sends a reply to the originator of the message.

func handoffReply(to: DispatchQueue, () -> Void) -> (any Encodable)?

Informs the system when message processing and response continues in a separate dispatch queue.

