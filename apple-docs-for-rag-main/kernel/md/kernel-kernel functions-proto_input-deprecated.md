

- Kernel
- Kernel Functions
-  proto_input Deprecated

Function

# proto_input

macOS 10.4–10.15.4Deprecated

``` source
errno_t proto_input(protocol_family_t protocol, mbuf_t packet);
```

## Parameters 

`protocol`  

The protocol of the packet.

`packet`  

The first packet in a chain of packets to be input.

## Return Value

A errno error on failure. Unless proto_input returns zero, the caller is responsible for freeing the mbuf.

## Discussion

Inputs a packet on the specified protocol from the input path.

