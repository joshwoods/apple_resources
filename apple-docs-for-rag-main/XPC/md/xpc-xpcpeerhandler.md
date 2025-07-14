

- XPC
-  XPCPeerHandler 

Protocol

# XPCPeerHandler

A type that handles incoming messages from a client and session cancellation.

Mac Catalyst 17.0+macOS 14.0+

``` source
protocol XPCPeerHandler
```

## Topics

### Receiving client messages

func handleIncomingRequest(Self.Input) -> Self.Output?

A closure that receives a message from a client and optionally provides a reply.

**Required**

associatedtype Input

A type that represents a message from a client.

**Required**

associatedtype Output

A type that represents a response to an incoming request.

**Required**

### Responding to session cancellation

func handleCancellation(error: XPCRichError)

A closure the system invokes when it cancels a session with a client.

**Required** Default implementation provided.

