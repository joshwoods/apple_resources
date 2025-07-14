

- Network Extension
- NEIPv4Route
-  gatewayAddress 

Instance Property

# gatewayAddress

The address of the next-hop gateway of the route.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var gatewayAddress: String? { get set }
```

## Discussion

The default value of this property is nil. When this property is nil, the route’s next-hop gateway will be set to the TUN interface unless it is a Split Exclude route.

## See Also

### Accessing IPv4 Route Properties

var destinationAddress: String

The destination network address of the route.

var destinationSubnetMask: String

The destination network mask of the route.

