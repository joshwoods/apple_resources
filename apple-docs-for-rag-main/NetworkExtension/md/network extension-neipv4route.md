

- Network Extension
-  NEIPv4Route 

Class

# NEIPv4Route

The settings for an IPv4 route.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEIPv4Route
```

## Mentioned in 

Routing your VPN network traffic

## Topics

### Creating an IPv4 Route

init(destinationAddress: String, subnetMask: String)

Initialize the NEIPv4Route object.

class func `default`() -> NEIPv4Route

A convenience method for creating the default IPv4 route.

### Accessing IPv4 Route Properties

var destinationAddress: String

The destination network address of the route.

var destinationSubnetMask: String

The destination network mask of the route.

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

var includedRoutes: [NEIPv4Route]?

The IPv4 network traffic that the system routes to the TUN interface.

var excludedRoutes: [NEIPv4Route]?

The IPv4 network traffic that the system routes to the primary physical interface, not the TUN interface.

