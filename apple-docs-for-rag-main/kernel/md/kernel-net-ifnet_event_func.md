

- Kernel
- net
-  ifnet_event_func 

Type Alias

# ifnet_event_func

macOS 10.4+

``` source
typedef void (*ifnet_event_func)(ifnet_t interface, const struct kev_msg *msg);
```

## Parameters 

`interface`  

The interface the event occurred on.

`event_ptr`  

Pointer to a kern_event structure describing the event.

## Discussion

ifnet_event_func is called when an event occurs on a specific interface.

## See Also

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_attach_proto_param_v2

ifnet_check_multi

ifnet_del_proto_func

ifnet_demux_desc

ifnet_demux_func

ifnet_detached_func

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

