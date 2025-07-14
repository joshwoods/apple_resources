

- vmnet
-  interface_param XPC Dictionary Keys 

API Collection

# interface_param XPC Dictionary Keys

XPC dictionary keys used by the `interface_param` argument returned by the completion handler of the `vmnet` function that describes the parameters that should be used to configure the network interface.

## Topics

### Constants

var vmnet_mac_address_key: UnsafePointer&lt;CChar>

var vmnet_mtu_key: UnsafePointer&lt;CChar>

var vmnet_max_packet_size_key: UnsafePointer&lt;CChar>

## See Also

### Constants

interface_desc XPC Dictionary Keys

XPC dictionary keys supported by the `interface_desc` parameter passed to the `vmnet` function to describe the parameters of the network interface.

event XPC Dictionary

XPC dictionary keys used by the `event` value returned to the client in the `handler` callback specified by the `vmnet` function that provides information about the callback event.

