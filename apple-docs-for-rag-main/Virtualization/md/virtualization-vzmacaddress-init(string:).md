

- Virtualization
- VZMACAddress
-  init(string:) 

Initializer

# init(string:)

Creates a MAC address object from a specially formatted string.

macOS 11.0+

``` source
convenience init?(string: String)
```

## Parameters 

`string`  

A string that contains the 6 hexadecimal bytes of the MAC address separated by colon characters. An example string is `01:23:45:ab:cd:ef`. The string is case-insensitive, so you may use uppercase or lowercase for alphabetical characters.

## Return Value

A MAC address object with the specified value, or `nil` if the string is formatted incorrectly.

## See Also

### Creating a MAC address

class func randomLocallyAdministered() -> Self

Returns a valid, random, locally administered, unicast MAC address.

init(ethernetAddress: ether_addr_t)

Creates a MAC address from the specified 48-bit Ethernet address.

