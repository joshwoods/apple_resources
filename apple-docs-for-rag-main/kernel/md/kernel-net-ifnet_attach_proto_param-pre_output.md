

- Kernel
- net
- ifnet_attach_proto_param
-  pre_output 

Instance Property

# pre_output

The function to be called for outbound packets.

macOS 10.6+

``` source
proto_media_preout pre_output;
```

## See Also

### Fields

demux_array

An array of ifnet_demux_desc structures describing the protocol.

demux_count

The number of entries in the demux_array array.

input

The function to be called for inbound packets.

event

The function to be called for interface events.

ioctl

The function to be called for ioctls.

detached

The function to be called for handling the detach.

