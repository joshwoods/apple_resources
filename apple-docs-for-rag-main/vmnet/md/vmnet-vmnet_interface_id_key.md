

- vmnet
-  vmnet_interface_id_key 

Global Variable

# vmnet_interface_id_key

Mac Catalyst 13.0+macOS 10.10+

``` source
var vmnet_interface_id_key: UnsafePointer
```

## Discussion

Interface identifier of the previously created interface.

If no interface identifier is passed to the `vmnet` function, a new MAC address is generated and a interface identifier is associated to it. This identifier is passed back to the client in the `interface_param` dictionary. To re-use a previously generated MAC address, the interface identifier associated with the MAC address needs to be passed to the `vmnet` function in the `interface_desc` parameter.

The value specified for this key should be of type doc://com.apple.documentation/documentation/xpc/xpc_type_uuid.

Important

Specifying a value for `vmnet_interface_id_key` does not guarantee the return of MAC address associated with the identifier. In cases where the MAC address associated with the id cannot be granted, an error is returned to the caller.

Note

This key may also be used in an XPC dictionary for a `interface_param` argument, for which it represents the identifier mapping to the MAC address returned in `vmnet_mac_address_key`. See interface_param XPC Dictionary Keys for more information.

## See Also

### Constants

var vmnet_operation_mode_key: UnsafePointer&lt;CChar>

