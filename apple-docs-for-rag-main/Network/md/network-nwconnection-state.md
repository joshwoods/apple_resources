

- Network
- NWConnection
-  state 

Instance Property

# state

The current state of the connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final var state: NWConnection.State { get }
```

## See Also

### Handling State Updates

enum State

States indicating whether a connection can be used to send and receive data.

var stateUpdateHandler: ((NWConnection.State) -> Void)?

A handler that receives connection state updates.

