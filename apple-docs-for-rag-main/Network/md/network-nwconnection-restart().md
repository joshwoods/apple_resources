

- Network
- NWConnection
-  restart() 

Instance Method

# restart()

Restarts a connection that is in the waiting state.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final func restart()
```

## Discussion

Restart a connection when it is in the waiting state and you have reason to believe the connection may succeed if it tries again. Connections that are waiting will automatically restart on network path changes.

## See Also

### Creating Connections

convenience init(host: NWEndpoint.Host, port: NWEndpoint.Port, using: NWParameters)

Initializes a new connection to a host and port.

init(to: NWEndpoint, using: NWParameters)

Initializes a new connection to a remote endpoint.

func start(queue: DispatchQueue)

Starts establishing a connection, and sets the queue on which to deliver all connection events.

