

- Kernel
- net
- ifnet_attach_proto_param
-  event 

Instance Property

# event

The function to be called for interface events.

macOS 10.6+

``` source
proto_media_event event;
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

ioctl

The function to be called for ioctls.

detached

The function to be called for handling the detach.

