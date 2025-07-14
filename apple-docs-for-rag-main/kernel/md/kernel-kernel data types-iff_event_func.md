

- Kernel
- Kernel Data Types
-  iff_event_func 

Type Alias

# iff_event_func

macOS 10.4+

``` source
typedef void (*iff_event_func)(void *cookie, ifnet_t interface, protocol_family_t protocol, const struct kev_msg *event_msg);
```

## Parameters 

`cookie`  

The cookie specified when this filter was attached.

`interface`  

The interface the packet is being transmitted on.

`event_msg`  

The kernel event, may not be changed.

## Discussion

iff_event_func is used to filter interface specific events. The interface is only valid for the duration of the filter call. If you need to keep a reference to the interface, be sure to call ifnet_reference and ifnet_release.

