

- XPC
- XPCReceivedMessage
-  handoffReply(to:\_:) 

Instance Method

# handoffReply(to:\_:)

Informs the system when message processing and response continues in a separate dispatch queue.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func handoffReply(
    to queue: DispatchQueue,
    _ continuation: @escaping () -> Void
) -> (any Encodable)?
```

## Parameters 

`queue`  

The dispatch queue where message processing continues. The queue must be an immutible queue hierarchy.

`continuation`  

The closure to perform on `queue`.

## Return Value

This method always returns `nil`, allowing a message handler closure to return a value.

## Discussion

You can only call this method from the context of a message handler closure, or from a continuation closure passed to handoffReply(to:_:).

## See Also

### Replying to messages

var expectsReply: Bool

A Boolean value that indicates if the client that sent the message expects a reply.

func reply&lt;Message>(Message)

Sends a reply to the originator of the message.

