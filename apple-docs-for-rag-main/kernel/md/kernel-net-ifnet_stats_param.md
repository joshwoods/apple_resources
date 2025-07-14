

- Kernel
- net
-  ifnet_stats_param 

# ifnet_stats_param

macOS 10.6+

``` source
struct ifnet_stats_param {
    ...
};
```

## Discussion

This structure is used get and set the interface statistics.

## Topics

### Fields

packets_in

The number of packets received.

bytes_in

The number of bytes received.

errors_in

The number of receive errors.

packets_out

The number of packets transmitted.

bytes_out

The number of bytes transmitted.

errors_out

The number of transmission errors.

collisions

The number of collisions seen by this interface.

dropped

The number of packets dropped.

### Instance Properties

multicasts_in

multicasts_out

no_protocol

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

ifnet_t

