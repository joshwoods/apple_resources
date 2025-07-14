

- Network Extension
- NEIPv4Settings
-  subnetMasks 

Instance Property

# subnetMasks

The IPv4 network masks to assign to the TUN interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var subnetMasks: [String] { get }
```

## Discussion

Each mask in this array is combined with the IP address in the corresponding index in `addresses` to specify an IPv4 network that the TUN interface is (virtually) connected to.

## See Also

### Accessing IPv4 properties

var addresses: [String]

The IPv4 addresses to assign to the TUN interface.

var router: String?

The address of the next-hop gateway router represented as a dotted decimal string.

