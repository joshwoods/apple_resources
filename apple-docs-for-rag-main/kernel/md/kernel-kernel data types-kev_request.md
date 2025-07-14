

- Kernel
- Kernel Data Types
-  kev_request 

# kev_request

macOS 10.9+

``` source
struct kev_request {
    ...
};
```

## Discussion

This structure is used with the SIOCSKEVFILT and SIOCGKEVFILT to set and get the control filter setting for a kernel control socket.

## Topics

### Fields

total_size

Total size of the kernel event message including the header.

vendor_code

All kernel events that don't match this vendor code will be ignored. KEV_ANY_VENDOR can be used to receive kernel events with any vendor code.

kev_class

All kernel events that don't match this class will be ignored. KEV_ANY_CLASS can be used to receive kernel events with any class.

kev_subclass

All kernel events that don't match this subclass will be ignored. KEV_ANY_SUBCLASS can be used to receive kernel events with any subclass.

