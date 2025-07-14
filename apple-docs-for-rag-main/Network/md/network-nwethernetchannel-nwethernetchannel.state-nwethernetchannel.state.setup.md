

- Network
- NWEthernetChannel
- NWEthernetChannel.State
-  NWEthernetChannel.State.setup 

Case

# NWEthernetChannel.State.setup

The channel has been initialized but not started.

macOS 10.15+

``` source
case setup
```

## See Also

### States

case waiting(NWError)

The channel is waiting for its interface to become available.

case preparing

The channel is registering with the interface.

case ready

The channel is able to send and receive Ethernet frames.

case failed(NWError)

The channel has encountered a fatal error.

case cancelled

The channel has been canceled.

