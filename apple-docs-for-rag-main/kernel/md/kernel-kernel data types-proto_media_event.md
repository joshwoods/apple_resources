

- Kernel
- Kernel Data Types
-  proto_media_event 

Type Alias

# proto_media_event

macOS 10.4+

``` source
typedef void (*proto_media_event)(ifnet_t ifp, protocol_family_t protocol, const struct kev_msg *event);
```

## Parameters 

`ifp`  

The interface.

`protocol_family`  

The protocol family.

`kev_msg`  

The event.

## Discussion

proto_media_event is called to notify this layer of interface specific events.

