

- Network
- IPv6Address
-  init(\_:) 

Initializer

# init(\_:)

Initializes an IPv6 address with a string.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init?(_ string: String)
```

## Discussion

The provided string will be interpreted as an IPv6 address. If the string cannot be interpreted as an IPv6 address, the initialization will fail.

## See Also

### Creating Addresses

init?(Data, NWInterface?)

Initializes an IPv6 address with data.

var asIPv4: IPv4Address?

Extracts the IPv4 address contained within the IPv6 address, if the IPv6 address is an IPv4-mapped or IPv4-compatible address.

