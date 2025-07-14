

- vmnet
-  vmnet_operation_mode_key 

Global Variable

# vmnet_operation_mode_key

Mac Catalyst 13.0+macOS 10.10+

``` source
var vmnet_operation_mode_key: UnsafePointer
```

## Discussion

The mode in which the guest operating system network interface is configured.

The supported modes are defined at `vmnet`.

The value specified for this key should be of type doc://com.apple.documentation/documentation/xpc/xpc_type_uint64.

## See Also

### Constants

var vmnet_interface_id_key: UnsafePointer&lt;CChar>

