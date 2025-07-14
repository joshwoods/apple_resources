

- Network
- NWListener
-  stateUpdateHandler 

Instance Property

# stateUpdateHandler

A handler that receives listener state updates.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
final var stateUpdateHandler: ((NWListener.State) -> Void)? { get set }
```

## See Also

### Creating Listeners

init(using: NWParameters, on: NWEndpoint.Port) throws

Initializes a network listener, with an optional local port.

func start(queue: DispatchQueue)

Registers for listening, and sets the queue on which all listener events are delivered.

enum State

States indicating whether a listener is able to accept incoming connections.

var port: NWEndpoint.Port?

The port on which the listener can accept connections.

func cancel()

Stops listening for inbound connections.

