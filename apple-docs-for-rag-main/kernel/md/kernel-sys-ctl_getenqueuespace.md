

- Kernel
- sys
-  ctl_getenqueuespace 

Function

# ctl_getenqueuespace

macOS 10.13+

``` source
errno_t ctl_getenqueuespace(kern_ctl_ref kctlref, u_int32_t unit, size_t *space);
```

## Parameters 

`kctlref`  

The control reference of the kernel control.

`unit`  

The unit number of the kernel control instance.

`space`  

The address where to return the current space available

## Return Value

0 - Success; the amount of space is returned to caller. EINVAL - Invalid parameters.

## Discussion

Retrieve the amount of space currently available for data to be sent from the kernel control to the client.

## See Also

### control

ctl_deregister

ctl_enqueuedata

ctl_enqueuembuf

ctl_getenqueuereadable

ctl_register

