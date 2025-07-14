

- Network
- NWConnection
- NWConnection.State
-  NWConnection.State.waiting(\_:) 

Case

# NWConnection.State.waiting(\_:)

The connection is waiting for a network path change.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case waiting(NWError)
```

## Discussion

Connections that are waiting will indicate the reason that the connection couldn’t be established in the associated error. These errors are not fatal.

## See Also

### States

case setup

The connection has been initialized but not started.

case preparing

The connection in the process of being established.

case ready

The connection is established, and ready to send and receive data.

case failed(NWError)

The connection has disconnected or encountered an error.

case cancelled

The connection has been canceled.

