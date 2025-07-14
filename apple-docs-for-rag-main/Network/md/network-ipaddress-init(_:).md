

- Network
- IPAddress
-  init(\_:) 

Initializer

# init(\_:)

Initializes an IP address with a string.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init?(_ string: String)
```

**Required**

## Discussion

The provided string will be interpreted as an IPv4 or IPv6 address. If the string cannot be interpreted as an address, the initialization will fail.

## See Also

### Creating Addresses

init?(Data, NWInterface?)

Initializes an IP address with data.

**Required**

