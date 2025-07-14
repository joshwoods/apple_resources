

- Kernel
- net
-  ifnet_ioctl_func 

Type Alias

# ifnet_ioctl_func

macOS 10.4+

``` source
typedef errno_t (*ifnet_ioctl_func)(ifnet_t interface, unsigned long cmd, void *data);
```

## Parameters 

`interface`  

The interface the ioctl is being sent to.

`proto_family`  

The protocol family to handle the ioctl, may be zero for no protocol_family.

`cmd`  

The ioctl command.

`data`  

A pointer to any data related to the ioctl.

## Discussion

ifnet_ioctl_func is used to communicate ioctls from the stack to the driver.

All undefined ioctls are reserved for future use by Apple. If you need to communicate with your kext using an ioctl, please use SIOCSIFKPI and SIOCGIFKPI.

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

ifnet_offload_t

Flags indicating the offload support of the interface.

ifnet_output_func

ifnet_set_bpf_tap

ifnet_stat_increment_param

ifnet_stats_param

ifnet_t

