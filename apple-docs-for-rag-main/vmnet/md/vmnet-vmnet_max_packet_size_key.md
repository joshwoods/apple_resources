

- vmnet
-  vmnet_max_packet_size_key 

Global Variable

# vmnet_max_packet_size_key

Mac Catalyst 13.0+macOS 10.10+

``` source
var vmnet_max_packet_size_key: UnsafePointer
```

## Discussion

The maximum size of the packet that can be written to the interface. This also defines the minimum size of the packet that needs to be passed to the `vmnet` function for a successful read.

The value for this key is of type doc://com.apple.documentation/documentation/xpc/xpc_type_uint64.

## See Also

### Constants

var vmnet_mac_address_key: UnsafePointer&lt;CChar>

var vmnet_mtu_key: UnsafePointer&lt;CChar>

