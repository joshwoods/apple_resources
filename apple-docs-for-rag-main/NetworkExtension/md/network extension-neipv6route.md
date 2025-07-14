

- Network Extension
-  NEIPv6Route 

Class

# NEIPv6Route

The settings for an IPv6 route.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEIPv6Route
```

## Mentioned in 

Routing your VPN network traffic

## Topics

### Creating an IPv6 Route

init(destinationAddress: String, networkPrefixLength: NSNumber)

Initialize the NEIPv6Route

class func `default`() -> NEIPv6Route

A convenience method for creating the default IPv4 route.

### Accessing IPv6 Route Properties

var destinationAddress: String

The destination network address of the route.

var destinationNetworkPrefixLength: NSNumber

The destination network prefix length of the route.

var gatewayAddress: String?

The address of the next-hop gateway of the route.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Routing network traffic

var includedRoutes: [NEIPv6Route]?

The IPv6 network traffic that the system routes to the TUN interface.

var excludedRoutes: [NEIPv6Route]?

The IPv6 network traffic that the system routes to the primary physical interface, not the TUN interface.

