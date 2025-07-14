

- Network
- NWEthernetChannel
- NWEthernetChannel.State
-  NWEthernetChannel.State.preparing 

Case

# NWEthernetChannel.State.preparing

The channel is registering with the interface.

macOS 10.15+

``` source
case preparing
```

## See Also

### States

case setup

The channel has been initialized but not started.

case waiting(NWError)

The channel is waiting for its interface to become available.

case ready

The channel is able to send and receive Ethernet frames.

case failed(NWError)

The channel has encountered a fatal error.

case cancelled

The channel has been canceled.

