

- Network Extension
- NEIPv4Route
-  destinationAddress 

Instance Property

# destinationAddress

The destination network address of the route.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var destinationAddress: String { get }
```

## Discussion

This string is combined with `destinationSubnetMask` to specify the destination network of the route.

## See Also

### Accessing IPv4 Route Properties

var destinationSubnetMask: String

The destination network mask of the route.

var gatewayAddress: String?

The address of the next-hop gateway of the route.

