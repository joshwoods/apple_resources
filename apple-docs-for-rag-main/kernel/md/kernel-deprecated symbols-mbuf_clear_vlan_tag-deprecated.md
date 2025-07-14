

- Kernel
- Deprecated Symbols
-  mbuf_clear_vlan_tag Deprecated

Function

# mbuf_clear_vlan_tag

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_clear_vlan_tag(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf containing the packet.

## Return Value

0 upon success otherwise the errno error.

## Discussion

This function will clear any vlan tag associated with the mbuf.

