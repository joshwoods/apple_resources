

- Network
- NWListener
- NWListener.State
-  NWListener.State.waiting(\_:) 

Case

# NWListener.State.waiting(\_:)

The listener is waiting for a network to become available.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case waiting(NWError)
```

## See Also

### States

case setup

The listener has been initialized but not started.

case ready

The listener is running and able to receive incoming connections.

case failed(NWError)

The listener has encountered a fatal error.

case cancelled

The listener has been canceled.

