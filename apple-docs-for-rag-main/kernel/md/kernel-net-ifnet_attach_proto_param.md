

- Kernel
- net
-  ifnet_attach_proto_param 

# ifnet_attach_proto_param

macOS 10.6+

``` source
struct ifnet_attach_proto_param {
    ...
};
```

## Discussion

This structure is used to attach a protocol to an interface. This structure provides the various functions for handling operations related to the protocol on the interface as well as information for how to demux packets for this protocol.

## Topics

### Fields

demux_array

An array of ifnet_demux_desc structures describing the protocol.

demux_count

The number of entries in the demux_array array.

input

The function to be called for inbound packets.

pre_output

The function to be called for outbound packets.

event

The function to be called for interface events.

ioctl

The function to be called for ioctls.

detached

The function to be called for handling the detach.

### Instance Properties

resolve

send_arp

## See Also

### ifnet

ifnet_add_proto_func

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

