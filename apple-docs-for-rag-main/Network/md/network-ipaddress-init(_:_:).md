

- Network
- IPAddress
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

Initializes an IP address with data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init?(
    _ rawValue: Data,
    _ interface: NWInterface?
)
```

**Required**

## Discussion

The provided data is expected to be either an IPv4 address of 4 bytes or an IPv6 address of 16 bytes.

## See Also

### Creating Addresses

init?(String)

Initializes an IP address with a string.

**Required**

