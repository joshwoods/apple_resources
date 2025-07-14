

- Network
- NWConnection
-  init(host:port:using:) 

Initializer

# init(host:port:using:)

Initializes a new connection to a host and port.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
convenience init(
    host: NWEndpoint.Host,
    port: NWEndpoint.Port,
    using: NWParameters
)
```

## See Also

### Creating Connections

init(to: NWEndpoint, using: NWParameters)

Initializes a new connection to a remote endpoint.

func start(queue: DispatchQueue)

Starts establishing a connection, and sets the queue on which to deliver all connection events.

func restart()

Restarts a connection that is in the waiting state.

