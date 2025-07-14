

- Network
- NWEthernetChannel
- NWEthernetChannel.State
-  NWEthernetChannel.State.failed(\_:) 

Case

# NWEthernetChannel.State.failed(\_:)

The channel has encountered a fatal error.

macOS 10.15+

``` source
case failed(NWError)
```

## See Also

### States

case setup

The channel has been initialized but not started.

case waiting(NWError)

The channel is waiting for its interface to become available.

case preparing

The channel is registering with the interface.

case ready

The channel is able to send and receive Ethernet frames.

case cancelled

The channel has been canceled.

