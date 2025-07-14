

- Kernel
- sys
-  sysctl_io_opaque 

Function

# sysctl_io_opaque

macOS 10.5+

``` source
int sysctl_io_opaque(struct sysctl_req *req, void *pValue, size_t valueSize, int *changed);
```

## See Also

### sysctl

sysctl_handle_int

sysctl_handle_int2quad

sysctl_handle_long

sysctl_handle_opaque

sysctl_handle_quad

sysctl_handle_string

sysctl_io_number

sysctl_io_string

sysctl_register_oid

sysctl_unregister_oid

sysctlbyname

Gets or sets information about the system and environment.

sysctl__children

sysctl__debug_children

sysctl__hw_children

sysctl__kern_children

sysctl__machdep_children

sysctl__net_children

sysctl__sysctl_children

sysctl__user_children

sysctl__vfs_children

sysctl__vm_children

