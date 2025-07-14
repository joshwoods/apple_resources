

- Network
- NWEthernetChannel
-  NWEthernetChannel.EthernetAddress 

Structure

# NWEthernetChannel.EthernetAddress

A 48-bit Ethernet address.

macOS 10.15+

``` source
struct EthernetAddress
```

## Topics

### Creating Addresses

init?(Data)

Initializes an Ethernet address with data.

init?(String)

Initializes an Ethernet address with a string.

### Inspecting Addresses

var rawValue: Data

The raw data of the Ethernet address.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Sending and Receiving Ethernet Frames

func send(content: Data, to: NWEthernetChannel.EthernetAddress, vlanTag: UInt16, completion: (NWError?) -> Void)

Sends a single Ethernet frame over a channel to a specific Ethernet address.

var receiveHandler: ((Data, UInt16, NWEthernetChannel.EthernetAddress, NWEthernetChannel.EthernetAddress) -> Void)?

A handler that delivers inbound Ethernet frames.

