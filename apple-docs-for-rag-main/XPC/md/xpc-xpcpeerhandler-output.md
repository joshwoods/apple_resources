

- XPC
- XPCPeerHandler
-  Output 

Associated Type

# Output

A type that represents a response to an incoming request.

Mac Catalyst 17.0+macOS 14.0+

``` source
associatedtype Output
```

**Required**

## See Also

### Receiving client messages

func handleIncomingRequest(Self.Input) -> Self.Output?

A closure that receives a message from a client and optionally provides a reply.

**Required**

associatedtype Input

A type that represents a message from a client.

**Required**

