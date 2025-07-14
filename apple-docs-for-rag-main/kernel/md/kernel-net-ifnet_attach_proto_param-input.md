

- Kernel
- net
- ifnet_attach_proto_param
-  input 

Instance Property

# input

The function to be called for inbound packets.

macOS 10.6+

``` source
proto_media_input input;
```

## See Also

### Fields

demux_array

An array of ifnet_demux_desc structures describing the protocol.

demux_count

The number of entries in the demux_array array.

pre_output

The function to be called for outbound packets.

event

The function to be called for interface events.

ioctl

The function to be called for ioctls.

detached

The function to be called for handling the detach.

