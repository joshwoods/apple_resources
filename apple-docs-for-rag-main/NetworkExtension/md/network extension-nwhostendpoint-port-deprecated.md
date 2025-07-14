

- Network Extension
- NWHostEndpoint
-  port Deprecated

Instance Property

# port

The endpoint’s port, represented as a string.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var port: String { get }
```

Deprecated

Use the nw_endpoint_get_port(_:) function from the Network framework instead.

## Discussion

Since the port is represented as a string, it is always represented in host byte order. If converting between byte fields and strings, make sure to use host byte ordering.

## See Also

### Getting endpoint properties

var hostname: String

The endpoint’s hostname.

Deprecated

