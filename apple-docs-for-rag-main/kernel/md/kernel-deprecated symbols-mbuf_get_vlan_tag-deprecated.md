

- Kernel
- Deprecated Symbols
-  mbuf_get_vlan_tag Deprecated

Function

# mbuf_get_vlan_tag

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_get_vlan_tag(mbuf_t mbuf, u_int16_t *vlan);
```

## Parameters 

`mbuf`  

The mbuf containing the packet.

`vlan`  

The protocol family of the aux data to add.

## Return Value

0 upon success otherwise the errno error. ENXIO indicates that the vlan tag is not set.

## Discussion

This function is used by drivers that support hardware vlan tagging to determine which vlan this packet belongs to. To differentiate between the case where the vlan tag is zero and the case where there is no vlan tag, this function will return ENXIO when there is no vlan.

