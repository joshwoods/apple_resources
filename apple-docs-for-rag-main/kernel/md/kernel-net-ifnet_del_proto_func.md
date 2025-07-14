

- Kernel
- net
-  ifnet_del_proto_func 

Type Alias

# ifnet_del_proto_func

macOS 10.4+

``` source
typedef errno_t (*ifnet_del_proto_func)(ifnet_t interface, protocol_family_t protocol_family);
```

## Parameters 

`interface`  

The interface the protocol will be detached from.

`protocol_family`  

The family of the protocol being detached.

## Return Value

If the result is zero, processing will continue normally. If the result is anything else, the detach will continue and the error will be returned to the caller.

## Discussion

if_del_proto_func is called by the stack when a protocol is being detached from an interface. This gives the interface an opportunity to free any storage related to this specific protocol being attached to this interface.

## See Also

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_attach_proto_param_v2

ifnet_check_multi

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

