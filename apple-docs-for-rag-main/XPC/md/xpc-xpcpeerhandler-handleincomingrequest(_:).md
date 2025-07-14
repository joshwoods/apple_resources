

- XPC
- XPCPeerHandler
-  handleIncomingRequest(\_:) 

Instance Method

# handleIncomingRequest(\_:)

A closure that receives a message from a client and optionally provides a reply.

Mac Catalyst 17.0+macOS 14.0+

``` source
func handleIncomingRequest(_: Self.Input) -> Self.Output?
```

**Required**

## Return Value

A response message, if any, to send back to the client; otherwise Nil.

## Discussion

If the closure returns Nil, you can still send use send(message:) to send an asynchronous reply after handling the message.

## See Also

### Receiving client messages

associatedtype Input

A type that represents a message from a client.

**Required**

associatedtype Output

A type that represents a response to an incoming request.

**Required**

