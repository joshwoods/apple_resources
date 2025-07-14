

- Network Extension
- NEIPv4Settings
-  router 

Instance Property

# router

The address of the next-hop gateway router represented as a dotted decimal string.

macOS 13.0+

``` source
var router: String? { get set }
```

## Discussion

The system ignores this property for TUN interfaces.

## See Also

### Accessing IPv4 properties

var addresses: [String]

The IPv4 addresses to assign to the TUN interface.

var subnetMasks: [String]

The IPv4 network masks to assign to the TUN interface.

