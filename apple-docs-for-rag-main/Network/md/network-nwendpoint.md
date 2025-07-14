

- Network
-  NWEndpoint 

Enumeration

# NWEndpoint

A local or remote endpoint in a network connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum NWEndpoint
```

## Topics

### Endpoint Types

case hostPort(host: NWEndpoint.Host, port: NWEndpoint.Port)

An endpoint represented as a host and port, with the host including both names and addresses.

case service(name: String, type: String, domain: String, interface: NWInterface?)

An endpoint represented as a Bonjour service.

case url(URL)

An endpoint represented as a URL, with host and port values inferred from the URL.

case unix(path: String)

An endpoint represented as a UNIX domain path.

### Host and Ports

enum Host

A name or address that identifies a network endpoint.

struct Port

A port number you use along with a host to identify a network endpoint.

### Internet Addresses

protocol IPAddress

An abstract protocol you use to interact with IP addresses.

struct IPv4Address

A structure containing an IPv4 address.

struct IPv6Address

A structure containing an IPv6 address.

### Endpoint Properties

var interface: NWInterface?

The optional interface associated with this endpoint, such as the interface on which it was discovered.

### Enumeration Cases

case opaque(nw_endpoint_t)

### Instance Properties

var txtRecord: NWTXTRecord?

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Essentials

class NWParameters

An object that stores the protocols to use for connections, options for sending data, and network path constraints.

