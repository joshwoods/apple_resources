

- Network
- NWEthernetChannel
-  cancel() 

Instance Method

# cancel()

Unregisters the channel from the interface.

macOS 10.15+

``` source
final func cancel()
```

## See Also

### Managing Ethernet Channels

init(on: NWInterface, etherType: UInt16)

Initializes an Ethernet channel on a specific interface with a custom Ethernet type.

func start(queue: DispatchQueue)

Starts the process of registering the channel, and sets the queue on which all channel events are delivered.

