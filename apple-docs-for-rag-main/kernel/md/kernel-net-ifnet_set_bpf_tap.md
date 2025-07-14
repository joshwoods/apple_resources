

- Kernel
- net
-  ifnet_set_bpf_tap 

Type Alias

# ifnet_set_bpf_tap

macOS 10.4+

``` source
typedef errno_t (*ifnet_set_bpf_tap)(ifnet_t interface, bpf_tap_mode mode, bpf_packet_func callback);
```

## Discussion

Deprecated. Specify NULL. Call bpf_tap_in/bpf_tap_out for all packets.

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

ifnet_stat_increment_param

ifnet_stats_param

ifnet_t

