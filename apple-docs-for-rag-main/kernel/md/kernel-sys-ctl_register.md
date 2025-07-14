

- Kernel
- sys
-  ctl_register 

Function

# ctl_register

macOS 10.13+

``` source
errno_t ctl_register(struct kern_ctl_reg *userkctl, kern_ctl_ref *kctlref);
```

## Parameters 

`userkctl`  

A structure defining the kernel control to be attached. The ctl_connect callback must be specified, the other callbacks are optional. If ctl_connect is set to zero, ctl_register fails with the error code EINVAL.

`kctlref`  

Upon successful return, the kctlref will contain a reference to the attached kernel control. This reference is used to unregister the kernel control. This reference will also be passed in to the callbacks each time they are called.

## Return Value

0 - Kernel control was registered. EINVAL - The registration structure was not valid. ENOMEM - There was insufficient memory. EEXIST - A controller with that id/unit is already registered.

## Discussion

Register a kernel control. This will enable clients to connect to the kernel control using a PF_SYSTEM socket.

## See Also

### control

ctl_deregister

ctl_enqueuedata

ctl_enqueuembuf

ctl_getenqueuereadable

ctl_getenqueuespace

