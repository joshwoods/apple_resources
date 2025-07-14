

- Kernel
- sys
-  ctl_deregister 

Function

# ctl_deregister

macOS 10.13+

``` source
errno_t ctl_deregister(kern_ctl_ref kctlref);
```

## Parameters 

`kctlref`  

The control reference of the control to unregister.

## Return Value

0 - Kernel control was unregistered. EINVAL - The kernel control reference was invalid. EBUSY - The kernel control has clients still attached.

## Discussion

Unregister a kernel control. A kernel extension must unregister it's kernel control(s) before unloading. If a kernel control has clients attached, this call will fail.

## See Also

### control

ctl_enqueuedata

ctl_enqueuembuf

ctl_getenqueuereadable

ctl_getenqueuespace

ctl_register

