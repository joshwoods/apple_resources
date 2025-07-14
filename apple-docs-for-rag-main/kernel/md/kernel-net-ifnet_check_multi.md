

- Kernel
- net
-  ifnet_check_multi 

Type Alias

# ifnet_check_multi

macOS 10.4+

``` source
typedef errno_t (*ifnet_check_multi)(ifnet_t interface, const struct sockaddr *mcast);
```

## Parameters 

`The`  

interface.

`mcast`  

The multicast address.

## Return Value

Zero upon success, EADDRNOTAVAIL on invalid multicast, EOPNOTSUPP for addresses the interface does not understand.

## Discussion

ifnet_check_multi is called for each multicast address added to an interface. This gives the interface an opportunity to reject invalid multicast addresses before they are attached to the interface.

To prevent an address from being added to your multicast list, return EADDRNOTAVAIL. If you don't know how to parse/translate the address, return EOPNOTSUPP.

## See Also

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_attach_proto_param_v2

ifnet_del_proto_func

ifnet_demux_desc

ifnet_demux_func

ifnet_detached_func

ifnet_event_func

ifnet_family_t

Storage type for the interface family.

ifnet_framer_func

ifnet_init_params

ifnet_ioctl_func

ifnet_offload_t

Flags indicating the offload support of the interface.

ifnet_output_func

ifnet_set_bpf_tap

ifnet_stat_increment_param

ifnet_stats_param

ifnet_t

