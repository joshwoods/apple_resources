

- Kernel
- Kernel Data Types
-  proto_plumb_handler 

Type Alias

# proto_plumb_handler

macOS 10.4+

``` source
typedef errno_t (*proto_plumb_handler)(ifnet_t ifp, protocol_family_t protocol);
```

## Parameters 

`ifp`  

The interface the protocol should be attached to.

`protocol_family`  

The protocol that should be attached to the interface.

## Return Value

A non-zero value of the attach failed.

## Discussion

proto_plumb_handler is called to attach a protocol to an interface. A typical protocol plumb function would fill out an ifnet_attach_proto_param and call ifnet_attach_protocol.

