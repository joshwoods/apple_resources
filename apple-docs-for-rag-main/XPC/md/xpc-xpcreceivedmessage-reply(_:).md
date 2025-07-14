

- XPC
- XPCReceivedMessage
-  reply(\_:) 

Instance Method

# reply(\_:)

Sends a reply to the originator of the message.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func reply(_ object: Message) where Message : Encodable
```

## Parameters 

`object`  

A message to send back to the client that sent the original message.

## Discussion

When a listener receives an XPCReceivedMessage, the message keeps track of the client that sent it. This function sends the specified reply message back to the originating client.

Don’t call this function more than once on a single message, and don’t call it on a message that wasn’t received from a client. Calling it more than once or sending a reply using a message that wasn’t received triggers an API misuse crash.

## See Also

### Replying to messages

var expectsReply: Bool

A Boolean value that indicates if the client that sent the message expects a reply.

func handoffReply(to: DispatchQueue, () -> Void) -> (any Encodable)?

Informs the system when message processing and response continues in a separate dispatch queue.

