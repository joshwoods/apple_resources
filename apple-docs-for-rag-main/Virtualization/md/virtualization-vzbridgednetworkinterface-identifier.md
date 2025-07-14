

- Virtualization
- VZBridgedNetworkInterface
-  identifier 

Instance Property

# identifier

The unique BSD name of this network interface.

macOS 11.0+

``` source
var identifier: String { get }
```

## Discussion

BSD names for the host computer’s Ethernet interfaces include `en0`, `en1`, and so on.

## See Also

### Getting the interface description

var localizedDisplayName: String?

A user-visible name for the network interface.

