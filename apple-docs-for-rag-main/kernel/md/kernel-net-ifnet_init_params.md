

- Kernel
- net
-  ifnet_init_params 

# ifnet_init_params

macOS 10.6+

``` source
struct ifnet_init_params {
    ...
};
```

## Discussion

This structure is used to define various properties of the interface when calling ifnet_allocate. A copy of these values will be stored in the ifnet and cannot be modified while the interface is attached.

## Topics

### Fields

uniqueid

An identifier unique to this instance of the interface.

uniqueid_len

The length, in bytes, of the uniqueid.

name

The interface name (i.e. en).

unit

The interface unit number (en0's unit number is 0).

family

The interface family.

type

The interface type (see sys/if_types.h). Must be less than 256. For new types, use IFT_OTHER.

output

The output function for the interface. Every packet the stack attempts to send through this interface will go out through this function.

demux

The function used to determine the protocol family of an incoming packet.

add_proto

The function used to attach a protocol to this interface.

del_proto

The function used to remove a protocol from this interface.

framer

The function used to frame outbound packets, may be NULL.

softc

Driver specific storage. This value can be retrieved from the ifnet using the ifnet_softc function.

ioctl

The function used to handle ioctls.

set_bpf_tap

The function used to set the bpf_tap function.

detach

The function called to let the driver know the interface has been detached.

event

The function to notify the interface of various interface specific kernel events.

broadcast_addr

The link-layer broadcast address for this interface.

broadcast_len

The length of the link-layer broadcast address.

### Instance Properties

check_multi

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

ifnet_ioctl_func

ifnet_offload_t

Flags indicating the offload support of the interface.

ifnet_output_func

ifnet_set_bpf_tap

ifnet_stat_increment_param

ifnet_stats_param

ifnet_t

