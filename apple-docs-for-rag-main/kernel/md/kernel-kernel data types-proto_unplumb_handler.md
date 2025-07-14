

- Kernel
- Kernel Data Types
-  proto_unplumb_handler 

Type Alias

# proto_unplumb_handler

macOS 10.4+

``` source
typedef void (*proto_unplumb_handler)(ifnet_t ifp, protocol_family_t protocol);
```

## Parameters 

`ifp`  

The interface the protocol should be detached from.

`protocol_family`  

The protocol that should be detached from the interface.

## Discussion

proto_unplumb_handler is called to detach a protocol from an interface. A typical unplumb function would call ifnet_detach_protocol and perform any necessary cleanup.

