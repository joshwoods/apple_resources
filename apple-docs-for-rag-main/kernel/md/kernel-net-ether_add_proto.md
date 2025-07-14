

- Kernel
- net
-  ether_add_proto 

Function

# ether_add_proto

macOS 10.4+

``` source
errno_t ether_add_proto(ifnet_t interface, protocol_family_t protocol, const struct ifnet_demux_desc *demux_list, u_int32_t demux_count);
```

## See Also

### ether

ether_family_init

ether_del_proto

ether_demux

ether_frameout

ether_ioctl

ether_check_multi

