

- Kernel
- Kernel Data Types
-  bpf_tap_func 

Type Alias

# bpf_tap_func

macOS 10.5+

``` source
typedef errno_t (*bpf_tap_func)(ifnet_t interface, u_int32_t data_link_type, bpf_tap_mode direction);
```

## Parameters 

`interface`  

The interface being tapped.

`dlt`  

The data link type being tapped.

`direction`  

The direction of the tap.

## Discussion

bpf_tap_func is called when the tap state of the interface changes. This happens when a bpf device attaches to an interface or detaches from an interface. The tap mode will join together (bit or) the modes of all bpf devices using that interface for that dlt. If you return an error from this function, the bpf device attach attempt that triggered the tap will fail. If this function was called bacuse the tap state was decreasing (tap in or out is stopping), the error will be ignored.

