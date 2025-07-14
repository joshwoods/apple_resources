

- Network
- NWEthernetChannel
- NWEthernetChannel.State
-  NWEthernetChannel.State.ready 

Case

# NWEthernetChannel.State.ready

The channel is able to send and receive Ethernet frames.

macOS 10.15+

``` source
case ready
```

## See Also

### States

case setup

The channel has been initialized but not started.

case waiting(NWError)

The channel is waiting for its interface to become available.

case preparing

The channel is registering with the interface.

case failed(NWError)

The channel has encountered a fatal error.

case cancelled

The channel has been canceled.

