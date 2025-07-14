

- Virtualization
- VZMACAddress
-  string 

Instance Property

# string

The MAC address as a formatted string.

macOS 11.0+

``` source
var string: String { get }
```

## Discussion

The string contains the 6 hexadecimal bytes of the MAC address, separated by colon characters. Alphabetical characters are lowercase in the string. An example string is `01:23:45:ab:cd:ef`.

## See Also

### Getting the address

var ethernetAddress: ether_addr_t

The MAC address as an Ethernet data structure.

