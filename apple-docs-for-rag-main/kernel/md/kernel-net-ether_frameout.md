

- Kernel
- net
-  ether_frameout 

Function

# ether_frameout

macOS 10.4+

``` source
errno_t ether_frameout(ifnet_t interface, mbuf_t *packet, const struct sockaddr *dest, const char *dest_lladdr, const char *frame_type);
```

## See Also

### ether

ether_family_init

ether_add_proto

ether_del_proto

ether_demux

ether_ioctl

ether_check_multi

