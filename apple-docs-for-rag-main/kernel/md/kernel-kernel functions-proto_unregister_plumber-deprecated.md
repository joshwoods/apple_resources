

- Kernel
- Kernel Functions
-  proto_unregister_plumber Deprecated

Function

# proto_unregister_plumber

macOS 10.4–10.15.4Deprecated

``` source
void proto_unregister_plumber(protocol_family_t proto_fam, ifnet_family_t if_fam);
```

## Parameters 

`proto_fam`  

The protocol family these plumbing functions handle.

`if_fam`  

The interface family these plumbing functions handle.

## Discussion

Unregisters a previously registered plumbing function.

