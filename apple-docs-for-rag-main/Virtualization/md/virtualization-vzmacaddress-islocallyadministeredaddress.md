

- Virtualization
- VZMACAddress
-  isLocallyAdministeredAddress 

Instance Property

# isLocallyAdministeredAddress

A Boolean value that indicates whether the address is a locally administered address (LAA).

macOS 11.0+

``` source
var isLocallyAdministeredAddress: Bool { get }
```

## Discussion

The value of this property is true if the address is locally administered, or false if it isn’t. A locally administered address different than the address burned in to the physical network interface.

## See Also

### Getting address attributes

var isBroadcastAddress: Bool

A Boolean value that indicates whether the address is a broadcast address.

var isMulticastAddress: Bool

A Boolean value that indicates whether the address is a multicast address.

var isUnicastAddress: Bool

A Boolean value that indicates whether the address is a unicast address.

var isUniversallyAdministeredAddress: Bool

A Boolean value that indicates whether the address is a universally adminstered address (UAA).

