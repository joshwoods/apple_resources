

- Kernel
- Kernel Functions
-  send_vfs_resolve_file 

Function

# send_vfs_resolve_file

macOS 12.0+

``` source
kern_return_t send_vfs_resolve_file(mach_port_t nspace_handler_port, uint32_t req_id, uint32_t pid, uint32_t op, int64_t offset, int64_t size, nspace_path_t path);
```

