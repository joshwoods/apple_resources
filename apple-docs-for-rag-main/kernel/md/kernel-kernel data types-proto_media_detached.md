

- Kernel
- Kernel Data Types
-  proto_media_detached 

Type Alias

# proto_media_detached

macOS 10.4+

``` source
typedef errno_t (*proto_media_detached)(ifnet_t ifp, protocol_family_t protocol);
```

## Parameters 

`ifp`  

The interface.

`protocol_family`  

The protocol family.

## Return Value

See the discussion.

## Discussion

proto_media_detached notifies you that your protocol has been detached.

