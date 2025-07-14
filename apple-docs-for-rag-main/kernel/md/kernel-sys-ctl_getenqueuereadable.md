

- Kernel
- sys
-  ctl_getenqueuereadable 

Function

# ctl_getenqueuereadable

macOS 10.13+

``` source
errno_t ctl_getenqueuereadable(kern_ctl_ref kctlref, u_int32_t unit, u_int32_t *difference);
```

## See Also

### control

ctl_deregister

ctl_enqueuedata

ctl_enqueuembuf

ctl_getenqueuespace

ctl_register

