

- Network
- NWConnection
-  stateUpdateHandler 

Instance Property

# stateUpdateHandler

A handler that receives connection state updates.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
final var stateUpdateHandler: ((NWConnection.State) -> Void)? { get set }
```

## See Also

### Handling State Updates

var state: NWConnection.State

The current state of the connection.

enum State

States indicating whether a connection can be used to send and receive data.

