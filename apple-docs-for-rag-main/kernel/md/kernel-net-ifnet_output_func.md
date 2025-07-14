

- Kernel
- net
-  ifnet_output_func 

Type Alias

# ifnet_output_func

macOS 10.4+

``` source
typedef errno_t (*ifnet_output_func)(ifnet_t interface, mbuf_t data);
```

## Parameters 

`interface`  

The interface being sent on.

`data`  

The packet to be sent.

## Discussion

ifnet_output_func is used to transmit packets. The stack will pass fully formed packets, including frame header, to the ifnet_output function for an interface. The driver is responsible for freeing the mbuf.

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

ifnet_set_bpf_tap

ifnet_stat_increment_param

ifnet_stats_param

ifnet_t

