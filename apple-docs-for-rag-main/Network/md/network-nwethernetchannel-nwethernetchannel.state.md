

- Network
- NWEthernetChannel
-  NWEthernetChannel.State 

Enumeration

# NWEthernetChannel.State

States indicating whether an Ethernet channel is able to send and receive frames.

macOS 10.15+

``` source
enum State
```

## Topics

### States

case setup

The channel has been initialized but not started.

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

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Handling State Updates

var state: NWEthernetChannel.State

The current state of the channel.

var stateUpdateHandler: ((NWEthernetChannel.State) -> Void)?

A handler that delivers channel state updates.

