

- Network
- NWEthernetChannel
-  receiveHandler 

Instance Property

# receiveHandler

A handler that delivers inbound Ethernet frames.

macOS 10.15+

``` source
@preconcurrency
final var receiveHandler: ((Data, UInt16, NWEthernetChannel.EthernetAddress, NWEthernetChannel.EthernetAddress) -> Void)? { get set }
```

## Discussion

The receive handler only needs to be set once, and will be invoked for each received Ethernet frame.

## See Also

### Sending and Receiving Ethernet Frames

func send(content: Data, to: NWEthernetChannel.EthernetAddress, vlanTag: UInt16, completion: (NWError?) -> Void)

Sends a single Ethernet frame over a channel to a specific Ethernet address.

struct EthernetAddress

A 48-bit Ethernet address.

