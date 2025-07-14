

- Network
- NWListener
-  cancel() 

Instance Method

# cancel()

Stops listening for inbound connections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final func cancel()
```

## See Also

### Creating Listeners

init(using: NWParameters, on: NWEndpoint.Port) throws

Initializes a network listener, with an optional local port.

func start(queue: DispatchQueue)

Registers for listening, and sets the queue on which all listener events are delivered.

var stateUpdateHandler: ((NWListener.State) -> Void)?

A handler that receives listener state updates.

enum State

States indicating whether a listener is able to accept incoming connections.

var port: NWEndpoint.Port?

The port on which the listener can accept connections.

