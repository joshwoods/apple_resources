

- Virtualization
- VZMACAddress
-  randomLocallyAdministered() 

Type Method

# randomLocallyAdministered()

Returns a valid, random, locally administered, unicast MAC address.

macOS 11.0+

``` source
class func randomLocallyAdministered() -> Self
```

## Return Value

A MAC address suitable for use in your network devices.

## Discussion

This method doesn’t guarantee the generation of a unique MAC address.

## See Also

### Creating a MAC address

convenience init?(string: String)

Creates a MAC address object from a specially formatted string.

init(ethernetAddress: ether_addr_t)

Creates a MAC address from the specified 48-bit Ethernet address.

