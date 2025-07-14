

- Network
- NWEthernetChannel
-  stateUpdateHandler 

Instance Property

# stateUpdateHandler

A handler that delivers channel state updates.

macOS 10.15+

``` source
@preconcurrency
final var stateUpdateHandler: ((NWEthernetChannel.State) -> Void)? { get set }
```

## See Also

### Handling State Updates

var state: NWEthernetChannel.State

The current state of the channel.

enum State

States indicating whether an Ethernet channel is able to send and receive frames.

