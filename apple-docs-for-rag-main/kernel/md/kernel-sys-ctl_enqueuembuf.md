

- Kernel
- sys
-  ctl_enqueuembuf 

Function

# ctl_enqueuembuf

macOS 10.13+

``` source
errno_t ctl_enqueuembuf(kern_ctl_ref kctlref, u_int32_t unit, mbuf_t m, u_int32_t flags);
```

## Parameters 

`kctlref`  

The control reference of the kernel control.

`unit`  

The unit number of the kernel control instance.

`m`  

An mbuf chain containing the data to send to the client.

`flags`  

Send flags. CTL_DATA_NOWAKEUP and CTL_DATA_EOR are currently the only supported flags.

## Return Value

0 - Data was enqueued to be read by the client. EINVAL - Invalid parameters. ENOBUFS - The queue is full.

## Discussion

Send data stored in an mbuf chain from the kernel control to the client. The caller is responsible for freeing the mbuf chain if ctl_enqueuembuf returns an error.

## See Also

### control

ctl_deregister

ctl_enqueuedata

ctl_getenqueuereadable

ctl_getenqueuespace

ctl_register

