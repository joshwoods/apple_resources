

- Kernel
- net
-  ether_ioctl 

Function

# ether_ioctl

macOS 10.4+

``` source
errno_t ether_ioctl(ifnet_t interface, u_int32_t command, void *data);
```

## See Also

### ether

ether_family_init

ether_add_proto

ether_del_proto

ether_demux

ether_frameout

ether_check_multi

