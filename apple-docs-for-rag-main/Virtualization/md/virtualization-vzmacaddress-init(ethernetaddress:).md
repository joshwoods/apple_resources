

- Virtualization
- VZMACAddress
-  init(ethernetAddress:) 

Initializer

# init(ethernetAddress:)

Creates a MAC address from the specified 48-bit Ethernet address.

macOS 11.0+

``` source
init(ethernetAddress: ether_addr_t)
```

## Parameters 

`ethernetAddress`  

A 48-bit Ethernet address.

## Return Value

A MAC address object with the specified Ethernet address.

## See Also

### Creating a MAC address

class func randomLocallyAdministered() -> Self

Returns a valid, random, locally administered, unicast MAC address.

convenience init?(string: String)

Creates a MAC address object from a specially formatted string.

