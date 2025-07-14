

- Network
- NWEthernetChannel
-  state 

Instance Property

# state

The current state of the channel.

macOS 10.15+

``` source
final var state: NWEthernetChannel.State { get }
```

## See Also

### Handling State Updates

enum State

States indicating whether an Ethernet channel is able to send and receive frames.

var stateUpdateHandler: ((NWEthernetChannel.State) -> Void)?

A handler that delivers channel state updates.

