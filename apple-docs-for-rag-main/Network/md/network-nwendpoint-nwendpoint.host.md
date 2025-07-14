

- Network
- NWEndpoint
-  NWEndpoint.Host 

Enumeration

# NWEndpoint.Host

A name or address that identifies a network endpoint.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum Host
```

## Topics

### Creating Hosts

init(String)

Initializes a host with a string.

### Accessing Host Types

case name(String, NWInterface?)

A host represented as a name.

case ipv4(IPv4Address)

A host represented as an IPv4 address.

case ipv6(IPv6Address)

A host represented as an IPv6 address.

### Requiring Interfaces

var interface: NWInterface?

The interface associated with this host, such as the interface scope stored in an IPv6 address.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

## See Also

### Host and Ports

struct Port

A port number you use along with a host to identify a network endpoint.

