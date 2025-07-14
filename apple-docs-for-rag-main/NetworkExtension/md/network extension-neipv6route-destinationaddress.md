

- Network Extension
- NEIPv6Route
-  destinationAddress 

Instance Property

# destinationAddress

The destination network address of the route.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var destinationAddress: String { get }
```

## Discussion

This string is combined with `destinationNetworkPrefixLength` to specify the destination network of the route.

## See Also

### Accessing IPv6 Route Properties

var destinationNetworkPrefixLength: NSNumber

The destination network prefix length of the route.

var gatewayAddress: String?

The address of the next-hop gateway of the route.

