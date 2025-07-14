

- Kernel
- Kernel Data Types
-  ctl_disconnect_func 

Type Alias

# ctl_disconnect_func

macOS 10.13+

``` source
typedef errno_t (*ctl_disconnect_func)(kern_ctl_ref kctlref, u_int32_t unit, void *unitinfo);
```

## Parameters 

`kctlref`  

The control ref for the kernel control instance the client has disconnected from.

`unit`  

The unit number of the kernel control instance the client has disconnected from.

`unitinfo`  

The user-defined private data initialized by the ctl_connect_func callback.

## Discussion

The ctl_disconnect_func is used to receive notification that a client has disconnected from the kernel control. This usually happens when the socket is closed. If this is the last socket attached to your kernel control, you may unregister your kernel control from this callback.

