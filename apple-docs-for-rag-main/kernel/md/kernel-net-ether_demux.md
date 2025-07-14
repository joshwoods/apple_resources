

- Kernel
- net
-  ether_demux 

Function

# ether_demux

macOS 10.4+

``` source
errno_t ether_demux(ifnet_t interface, mbuf_t packet, char *header, protocol_family_t *protocol);
```

## See Also

### ether

ether_family_init

ether_add_proto

ether_del_proto

ether_frameout

ether_ioctl

ether_check_multi

