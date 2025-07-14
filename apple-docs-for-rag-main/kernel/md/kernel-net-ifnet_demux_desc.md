

- Kernel
- net
-  ifnet_demux_desc 

# ifnet_demux_desc

macOS 10.6+

``` source
struct ifnet_demux_desc {
    ...
};
```

## Discussion

This structure is to identify packets that belong to a specific protocol. The types supported are interface specific. Ethernet supports ETHER_DESC_ETYPE2, ETHER_DESC_SAP, and ETHER_DESC_SNAP. The type defines the offset in the packet where the data will be matched as well as context. For example, if ETHER_DESC_SNAP is specified, the only valid datalen is 5 and only in the 5 bytes will only be matched when the packet header indicates that the packet is a SNAP packet.

## Topics

### Fields

type

The type of identifier data (i.e. ETHER_DESC_ETYPE2)

data

A pointer to an entry of type (i.e. pointer to 0x0800).

datalen

The number of bytes of data used to describe the packet.

## See Also

### ifnet

ifnet_add_proto_func

ifnet_attach_proto_param

ifnet_attach_proto_param_v2

ifnet_check_multi

ifnet_del_proto_func

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

