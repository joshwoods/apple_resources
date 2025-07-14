

- XPC
- XPCPeerHandler
-  Input 

Associated Type

# Input

A type that represents a message from a client.

Mac Catalyst 17.0+macOS 14.0+

``` source
associatedtype Input
```

**Required**

## See Also

### Receiving client messages

func handleIncomingRequest(Self.Input) -> Self.Output?

A closure that receives a message from a client and optionally provides a reply.

**Required**

associatedtype Output

A type that represents a response to an incoming request.

**Required**

