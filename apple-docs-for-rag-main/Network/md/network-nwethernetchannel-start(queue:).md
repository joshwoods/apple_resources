

- Network
- NWEthernetChannel
-  start(queue:) 

Instance Method

# start(queue:)

Starts the process of registering the channel, and sets the queue on which all channel events are delivered.

macOS 10.15+

``` source
final func start(queue: DispatchQueue)
```

## See Also

### Managing Ethernet Channels

init(on: NWInterface, etherType: UInt16)

Initializes an Ethernet channel on a specific interface with a custom Ethernet type.

func cancel()

Unregisters the channel from the interface.

