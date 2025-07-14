

- Virtualization
- VZBridgedNetworkInterface
-  localizedDisplayName 

Instance Property

# localizedDisplayName

A user-visible name for the network interface.

macOS 11.0+

``` source
var localizedDisplayName: String? { get }
```

## Discussion

An example interface name is `Ethernet`. Use this string when you need to display the name of the interface to the user.

## See Also

### Getting the interface description

var identifier: String

The unique BSD name of this network interface.

