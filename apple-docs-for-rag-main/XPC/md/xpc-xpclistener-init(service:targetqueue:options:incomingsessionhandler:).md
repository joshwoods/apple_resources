

- XPC
- XPCListener
-  init(service:targetQueue:options:incomingSessionHandler:) 

Initializer

# init(service:targetQueue:options:incomingSessionHandler:)

Creates the server side of an XPC service using the specified service name.

Mac Catalyst 17.0+macOS 14.0+

``` source
init(
    service: String,
    targetQueue: DispatchQueue? = nil,
    options: XPCListener.InitializationOptions = .none,
    incomingSessionHandler: @escaping (XPCListener.IncomingSessionRequest) -> XPCListener.IncomingSessionRequest.Decision
) throws
```

## Parameters 

`service`  

The Mach service or XPC service name that clients use to connect to the service.

`targetQueue`  

The dispatch queue that events arrive on. This may be a concurrent queue. If Nil, the listeners uses `DISPATCH_TARGET_QUEUE_DEFAULT`.

`options`  

Configuration options for the listener, such as creating it in an inactive state.

`incomingSessionHandler`  

A handler that the system calls when a client connects to the XPC service.

## Discussion

Listener creation fails if the XPC service isn’t found or is unavailable.

When a client connects to your service, the system invokes the `incomingSessionHandler` with a request that you must either accept or reject. To accept the incoming request, choose one of the following two approaches:

- For simple protocols, use accept(incomingMessageHandler:cancellationHandler:) or accept(incomingMessageHandler:cancellationHandler:) to provide a closure that receives the incoming message directly.

- For more complex protocols that delegate message handling to a different object, use `accept(_:)` to provide a closure that returns a XPCPeerHandler. The peer handler object receives incoming messages from the client directly.

When the `incomingSessionHandler` returns, the system automatically activates the peer session unless you explicitly reject it or pass the inactive initialzation option.

## See Also

### Creating a listener

struct InitializationOptions

Options that control the listener’s configuration, such as if it’s inactive at creation.

class IncomingSessionRequest

A session request from a client that you accept or reject.

