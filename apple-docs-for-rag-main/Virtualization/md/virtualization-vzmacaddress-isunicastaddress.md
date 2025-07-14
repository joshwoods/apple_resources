

- Virtualization
- VZMACAddress
-  isUnicastAddress 

Instance Property

# isUnicastAddress

A Boolean value that indicates whether the address is a unicast address.

macOS 11.0+

``` source
var isUnicastAddress: Bool { get }
```

## Discussion

The value of this property is true if the address is a unicast address, or false if it isn’t.

## See Also

### Getting address attributes

var isBroadcastAddress: Bool

A Boolean value that indicates whether the address is a broadcast address.

var isMulticastAddress: Bool

A Boolean value that indicates whether the address is a multicast address.

var isLocallyAdministeredAddress: Bool

A Boolean value that indicates whether the address is a locally administered address (LAA).

var isUniversallyAdministeredAddress: Bool

A Boolean value that indicates whether the address is a universally adminstered address (UAA).

