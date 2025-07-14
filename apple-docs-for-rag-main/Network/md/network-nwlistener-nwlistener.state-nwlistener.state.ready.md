

- Network
- NWListener
- NWListener.State
-  NWListener.State.ready 

Case

# NWListener.State.ready

The listener is running and able to receive incoming connections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case ready
```

## See Also

### States

case setup

The listener has been initialized but not started.

case waiting(NWError)

The listener is waiting for a network to become available.

case failed(NWError)

The listener has encountered a fatal error.

case cancelled

The listener has been canceled.

