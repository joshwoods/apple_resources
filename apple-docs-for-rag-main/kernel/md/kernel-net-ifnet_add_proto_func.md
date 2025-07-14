

- Kernel
- net
-  ifnet_add_proto_func 

Type Alias

# ifnet_add_proto_func

macOS 10.4+

``` source
typedef errno_t (*ifnet_add_proto_func)(ifnet_t interface, protocol_family_t protocol_family, const struct ifnet_demux_desc *demux_array, u_int32_t demux_count);
```

## Parameters 

`interface`  

The interface the protocol will be attached to.

`protocol_family`  

The family of the protocol being attached.

`demux_array`  

An array of demux descriptors that describe the interface specific ways of identifying packets belonging to this protocol family.

`demux_count`  

The number of demux descriptors in the array.

## Return Value

If the result is zero, processing will continue normally. If the result is anything else, the add protocol will be aborted.

## Discussion

if_add_proto_func is called by the stack when a protocol is attached to an interface. This gives the interface an opportunity to get a list of protocol description structures for demuxing packets to this protocol (demux descriptors).

## See Also

### ifnet

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

ifnet_stats_param

ifnet_t

