

- Kernel
- sys
-  ctl_enqueuedata 

Function

# ctl_enqueuedata

macOS 10.13+

``` source
errno_t ctl_enqueuedata(kern_ctl_ref kctlref, u_int32_t unit, void *data, size_t len, u_int32_t flags);
```

## Parameters 

`kctlref`  

The control reference of the kernel control.

`unit`  

The unit number of the kernel control instance.

`data`  

A pointer to the data to send.

`len`  

The length of data to send.

`flags`  

Send flags. CTL_DATA_NOWAKEUP and CTL_DATA_EOR are currently the only supported flags.

## Return Value

0 - Data was enqueued to be read by the client. EINVAL - Invalid parameters. EMSGSIZE - The buffer is too large. ENOBUFS - The queue is full or there are no free mbufs.

## Discussion

Send data from the kernel control to the client.

## See Also

### control

ctl_deregister

ctl_enqueuembuf

ctl_getenqueuereadable

ctl_getenqueuespace

ctl_register

