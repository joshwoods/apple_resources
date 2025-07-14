

- Kernel
- Kernel Functions
-  proto_inject Deprecated

Function

# proto_inject

macOS 10.4–10.15.4Deprecated

``` source
errno_t proto_inject(protocol_family_t protocol, mbuf_t packet);
```

## Parameters 

`protocol`  

The protocol of the packet.

`packet`  

The first packet in a chain of packets to be injected.

## Return Value

A errno error on failure. Unless proto_inject returns zero, the caller is responsible for freeing the mbuf.

## Discussion

Injects a packet on the specified protocol from anywhere. To avoid recursion, the protocol may need to queue the packet to be handled later.

