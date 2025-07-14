

- Kernel
- net
-  ifnet_detached_func 

Type Alias

# ifnet_detached_func

macOS 10.4+

``` source
typedef void (*ifnet_detached_func)(ifnet_t interface);
```

## Parameters 

`interface`  

The interface that has been detached. event.

## Discussion

ifnet_detached_func is called an interface is detached from the list of interfaces. When ifnet_detach is called, it may not detach the interface immediately if protocols are attached. ifnet_detached_func is used to notify the interface that it has been detached from the networking stack. This is the last function that will be called on an interface. Until this function returns, you must not unload a kext supplying function pointers to this interface, even if ifnet_detacah has been called. Your detach function may be called during your call to ifnet_detach.

## See Also

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_attach_proto_param_v2

ifnet_check_multi

ifnet_del_proto_func

ifnet_demux_desc

ifnet_demux_func

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

