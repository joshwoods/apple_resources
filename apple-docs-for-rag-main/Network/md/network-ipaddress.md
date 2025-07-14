

- Network
-  IPAddress 

Protocol

# IPAddress

An abstract protocol you use to interact with IP addresses.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
protocol IPAddress : Sendable
```

## Topics

### Creating Addresses

init?(String)

Initializes an IP address with a string.

**Required**

init?(Data, NWInterface?)

Initializes an IP address with data.

**Required**

### Inspecting Address Properties

var rawValue: Data

The raw data of an IP address.

**Required**

var interface: NWInterface?

The interface associated with this address, such as the IPv6 scoped interface.

**Required**

var isLinkLocal: Bool

A Boolean indicating whether this address is in a link-local range.

**Required**

var isLoopback: Bool

A Boolean indicating whether this address is a loopback address for the local device.

**Required**

var isMulticast: Bool

A Boolean indicating whether this address is a multicast address.

**Required**

## Relationships

### Inherits From

- Sendable

### Conforming Types

- IPv4Address
- IPv6Address

## See Also

### Internet Addresses

struct IPv4Address

A structure containing an IPv4 address.

struct IPv6Address

A structure containing an IPv6 address.

