

- Network
- IPv4Address
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

Initializes an IPv4 address with data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init?(
    _ rawValue: Data,
    _ interface: NWInterface? = nil
)
```

## Discussion

The provided data is expected to be an IPv4 address of 4 bytes.

## See Also

### Creating Addresses

init?(String)

Initializes an IPv4 address with a string.

