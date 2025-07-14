

- Network
-  IPv4Address 

Structure

# IPv4Address

A structure containing an IPv4 address.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct IPv4Address
```

## Topics

### Creating Addresses

init?(String)

Initializes an IPv4 address with a string.

init?(Data, NWInterface?)

Initializes an IPv4 address with data.

### Inspecting Address Properties

var rawValue: Data

The raw data of an IPv4 address.

let interface: NWInterface?

The interface associated with this address.

var isLinkLocal: Bool

A Boolean indicating whether this address is in a link-local range.

var isLoopback: Bool

A Boolean indicating whether this address is a loopback address for the local device.

var isMulticast: Bool

A Boolean indicating whether this address is a multicast address.

### Setting Well-Known Addresses

static let any: IPv4Address

The unspecified address (0.0.0.0).

static let broadcast: IPv4Address

The local broadcast address (255.255.255.255).

static let loopback: IPv4Address

The device’s loopback address (127.0.0.1).

static let allHostsGroup: IPv4Address

The multicast group for all hosts on the network segment (224.0.0.1).

static let allRoutersGroup: IPv4Address

The multicast group for all routers on the network segment (224.0.0.2).

static let allReportsGroup: IPv4Address

The multicast group for all IGMPv3 reports (224.0.0.22).

static let mdnsGroup: IPv4Address

The multicast group for multicast DNS (224.0.0.251).

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- IPAddress
- Sendable

## See Also

### Internet Addresses

protocol IPAddress

An abstract protocol you use to interact with IP addresses.

struct IPv6Address

A structure containing an IPv6 address.

