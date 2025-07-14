

- Network
- NWConnection
-  NWConnection.State 

Enumeration

# NWConnection.State

States indicating whether a connection can be used to send and receive data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum State
```

## Topics

### States

case setup

The connection has been initialized but not started.

case waiting(NWError)

The connection is waiting for a network path change.

case preparing

The connection in the process of being established.

case ready

The connection is established, and ready to send and receive data.

case failed(NWError)

The connection has disconnected or encountered an error.

case cancelled

The connection has been canceled.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Handling State Updates

var state: NWConnection.State

The current state of the connection.

var stateUpdateHandler: ((NWConnection.State) -> Void)?

A handler that receives connection state updates.

