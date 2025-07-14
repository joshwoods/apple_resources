

- Network
- IPv6Address
-  asIPv4 

Instance Property

# asIPv4

Extracts the IPv4 address contained within the IPv6 address, if the IPv6 address is an IPv4-mapped or IPv4-compatible address.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var asIPv4: IPv4Address? { get }
```

## See Also

### Creating Addresses

init?(String)

Initializes an IPv6 address with a string.

init?(Data, NWInterface?)

Initializes an IPv6 address with data.

