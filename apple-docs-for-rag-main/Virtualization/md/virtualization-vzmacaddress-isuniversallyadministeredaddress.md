

- Virtualization
- VZMACAddress
-  isUniversallyAdministeredAddress 

Instance Property

# isUniversallyAdministeredAddress

A Boolean value that indicates whether the address is a universally adminstered address (UAA).

macOS 11.0+

``` source
var isUniversallyAdministeredAddress: Bool { get }
```

## Discussion

The value of this property is true if the address is universally administered, or false if it isn’t. The manufacturer of a device assigns an address of this type, and the address includes the organization’s unique identification code.

## See Also

### Getting address attributes

var isBroadcastAddress: Bool

A Boolean value that indicates whether the address is a broadcast address.

var isMulticastAddress: Bool

A Boolean value that indicates whether the address is a multicast address.

var isUnicastAddress: Bool

A Boolean value that indicates whether the address is a unicast address.

var isLocallyAdministeredAddress: Bool

A Boolean value that indicates whether the address is a locally administered address (LAA).

