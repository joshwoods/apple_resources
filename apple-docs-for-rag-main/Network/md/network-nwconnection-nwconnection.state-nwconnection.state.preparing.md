

- Network
- NWConnection
- NWConnection.State
-  NWConnection.State.preparing 

Case

# NWConnection.State.preparing

The connection in the process of being established.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case preparing
```

## See Also

### States

case setup

The connection has been initialized but not started.

case waiting(NWError)

The connection is waiting for a network path change.

case ready

The connection is established, and ready to send and receive data.

case failed(NWError)

The connection has disconnected or encountered an error.

case cancelled

The connection has been canceled.

