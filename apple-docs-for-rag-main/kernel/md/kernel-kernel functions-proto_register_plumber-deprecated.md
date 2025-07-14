

- Kernel
- Kernel Functions
-  proto_register_plumber Deprecated

Function

# proto_register_plumber

macOS 10.4–10.15.4Deprecated

``` source
errno_t proto_register_plumber(protocol_family_t proto_fam, ifnet_family_t if_fam, proto_plumb_handler plumb, proto_unplumb_handler unplumb);
```

## Parameters 

`proto_fam`  

The protocol family these plumbing functions will handle.

`if_fam`  

The interface family these plumbing functions will handle.

`plumb`  

The function to call to attach the protocol to an interface.

`unplumb`  

The function to call to detach the protocol to an interface, may be NULL in which case ifnet_detach_protocol will be used to detach the protocol.

## Return Value

A non-zero value of the attach failed.

## Discussion

Allows the caller to specify the functions called when a protocol is attached to an interface belonging to the specified family and when that protocol is detached.

