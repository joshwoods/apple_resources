

- Kernel
- net
- ifnet_attach_proto_param
-  detached 

Instance Property

# detached

The function to be called for handling the detach.

macOS 10.6+

``` source
proto_media_detached detached;
```

## See Also

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

