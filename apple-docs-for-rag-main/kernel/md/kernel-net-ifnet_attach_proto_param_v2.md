

- Kernel
- net
-  ifnet_attach_proto_param_v2 

# ifnet_attach_proto_param_v2

macOS 10.6+

``` source
struct ifnet_attach_proto_param_v2 {
    ...
};
```

## Topics

### Instance Properties

demux_array

demux_count

detached

event

input

ioctl

pre_output

resolve

send_arp

## See Also

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_check_multi

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

