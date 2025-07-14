

- vmnet
-  interface_desc XPC Dictionary Keys 

API Collection

# interface_desc XPC Dictionary Keys

XPC dictionary keys supported by the `interface_desc` parameter passed to the `vmnet` function to describe the parameters of the network interface.

## Topics

### Constants

var vmnet_operation_mode_key: UnsafePointer&lt;CChar>

var vmnet_interface_id_key: UnsafePointer&lt;CChar>

## See Also

### Constants

interface_param XPC Dictionary Keys

XPC dictionary keys used by the `interface_param` argument returned by the completion handler of the `vmnet` function that describes the parameters that should be used to configure the network interface.

event XPC Dictionary

XPC dictionary keys used by the `event` value returned to the client in the `handler` callback specified by the `vmnet` function that provides information about the callback event.

