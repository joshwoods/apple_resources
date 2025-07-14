

- Network
- NWEthernetChannel
-  send(content:to:vlanTag:completion:) 

Instance Method

# send(content:to:vlanTag:completion:)

Sends a single Ethernet frame over a channel to a specific Ethernet address.

macOS 10.15+

``` source
@preconcurrency
final func send(
    content: Data,
    to remoteAddress: NWEthernetChannel.EthernetAddress,
    vlanTag: UInt16,
    completion: @escaping (NWError?) -> Void
)
```

## See Also

### Sending and Receiving Ethernet Frames

var receiveHandler: ((Data, UInt16, NWEthernetChannel.EthernetAddress, NWEthernetChannel.EthernetAddress) -> Void)?

A handler that delivers inbound Ethernet frames.

struct EthernetAddress

A 48-bit Ethernet address.

