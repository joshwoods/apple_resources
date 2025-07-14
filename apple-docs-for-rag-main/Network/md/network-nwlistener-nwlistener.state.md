

- Network
- NWListener
-  NWListener.State 

Enumeration

# NWListener.State

States indicating whether a listener is able to accept incoming connections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum State
```

## Topics

### States

case setup

The listener has been initialized but not started.

case waiting(NWError)

The listener is waiting for a network to become available.

case ready

The listener is running and able to receive incoming connections.

case failed(NWError)

The listener has encountered a fatal error.

case cancelled

The listener has been canceled.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Creating Listeners

init(using: NWParameters, on: NWEndpoint.Port) throws

Initializes a network listener, with an optional local port.

func start(queue: DispatchQueue)

Registers for listening, and sets the queue on which all listener events are delivered.

var stateUpdateHandler: ((NWListener.State) -> Void)?

A handler that receives listener state updates.

var port: NWEndpoint.Port?

The port on which the listener can accept connections.

func cancel()

Stops listening for inbound connections.

