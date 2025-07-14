

- Kernel
- net
-  ifnet_demux_func 

Type Alias

# ifnet_demux_func

macOS 10.4+

``` source
typedef errno_t (*ifnet_demux_func)(ifnet_t interface, mbuf_t packet, char *frame_header, protocol_family_t *protocol_family);
```

## Parameters 

`interface`  

The interface the packet was received on.

`packet`  

The mbuf containing the packet.

`frame_header`  

A pointer to the frame header.

`protocol_family`  

Upon return, the protocol family matching the packet should be stored here.

## Return Value

If the result is zero, processing will continue normally. If the result is EJUSTRETURN, processing will stop but the packet will not be freed. If the result is anything else, the processing will stop and the packet will be freed.

## Discussion

ifnet_demux_func is called for each inbound packet to determine which protocol family the packet belongs to. This information is then used by the stack to determine which protocol to pass the packet to. This function may return protocol families for protocols that are not attached. If the protocol family has not been attached to the interface, the packet will be discarded.

## See Also

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_attach_proto_param_v2

ifnet_check_multi

ifnet_del_proto_func

ifnet_demux_desc

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

