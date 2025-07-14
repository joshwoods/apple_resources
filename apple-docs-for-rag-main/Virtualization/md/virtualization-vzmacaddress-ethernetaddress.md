

- Virtualization
- VZMACAddress
-  ethernetAddress 

Instance Property

# ethernetAddress

The MAC address as an Ethernet data structure.

macOS 11.0+

``` source
var ethernetAddress: ether_addr_t { get }
```

## Discussion

Use this property to obtain the individual octets of the Ethernet address. For more information, see `ether_addr_t`.

## See Also

### Getting the address

var string: String

The MAC address as a formatted string.

