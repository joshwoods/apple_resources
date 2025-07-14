

- Network
- NWEthernetChannel
-  init(on:etherType:) 

Initializer

# init(on:etherType:)

Initializes an Ethernet channel on a specific interface with a custom Ethernet type.

macOS 10.15+

``` source
init(
    on interface: NWInterface,
    etherType: UInt16
)
```

## Parameters 

`interface`  

The interface on which to send and receive Ethernet frames.

`etherType`  

The custom Ethernet frame type to register for this channel, in host-byte order.

## See Also

### Managing Ethernet Channels

func start(queue: DispatchQueue)

Starts the process of registering the channel, and sets the queue on which all channel events are delivered.

func cancel()

Unregisters the channel from the interface.

