

- Network
- NWEthernetChannel
- NWEthernetChannel.State
-  NWEthernetChannel.State.waiting(\_:) 

Case

# NWEthernetChannel.State.waiting(\_:)

The channel is waiting for its interface to become available.

macOS 10.15+

``` source
case waiting(NWError)
```

## See Also

### States

case setup

The channel has been initialized but not started.

case preparing

The channel is registering with the interface.

case ready

The channel is able to send and receive Ethernet frames.

case failed(NWError)

The channel has encountered a fatal error.

case cancelled

The channel has been canceled.

