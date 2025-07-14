

- Kernel
- net
- ifnet_attach_proto_param
-  demux_count 

Instance Property

# demux_count

The number of entries in the demux_array array.

macOS 10.6+

``` source
u_int32_t demux_count;
```

## See Also

### Fields

demux_array

An array of ifnet_demux_desc structures describing the protocol.

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

