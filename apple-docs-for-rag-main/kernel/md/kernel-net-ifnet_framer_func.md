

- Kernel
- net
-  ifnet_framer_func 

Type Alias

# ifnet_framer_func

macOS 10.4+

``` source
typedef errno_t (*ifnet_framer_func)(ifnet_t interface, mbuf_t *packet, const struct sockaddr *dest, const char *dest_linkaddr, const char *frame_type);
```

## Parameters 

`interface`  

The interface the packet is being sent on.

`packet`  

Pointer to the mbuf containing the packet, caller may set this to a different mbuf upon return. This can happen if the frameout function needs to prepend another mbuf to the chain to have enough space for the header.

`dest`  

The higher layer protocol destination (i.e. IP address).

`dest_linkaddr`  

The link layer address as determined by the protocol's pre-output function.

`frame_type`  

The frame type as determined by the protocol's pre-output function.

`prepend_len`  

The length of prepended bytes to the mbuf. (ONLY used if KPI_INTERFACE_EMBEDDED is defined to 1)

`postpend_len`  

The length of the postpended bytes to the mbuf. (ONLY used if KPI_INTERFACE_EMBEDDED is defined to 1)

## Return Value

If the result is zero, processing will continue normally. If the result is EJUSTRETURN, processing will stop but the packet will not be freed. If the result is anything else, the processing will stop and the packet will be freed.

## Discussion

ifnet_framer_func is called for each outbound packet to give the interface an opportunity to prepend interface specific headers.

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

ifnet_init_params

ifnet_ioctl_func

ifnet_offload_t

Flags indicating the offload support of the interface.

ifnet_output_func

ifnet_set_bpf_tap

ifnet_stat_increment_param

ifnet_stats_param

ifnet_t

