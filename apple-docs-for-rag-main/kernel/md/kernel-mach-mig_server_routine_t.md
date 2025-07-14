

- Kernel
- mach
-  mig_server_routine_t 

Type Alias

# mig_server_routine_t

macOS 10.1+

``` source
typedef mig_routine_t (*mig_server_routine_t)(mach_msg_header_t *InHeadP);
```

## See Also

### MIG

mig_allocate

mig_dealloc_reply_port

mig_deallocate

mig_get_reply_port

mig_put_reply_port

mig_strncpy

mig_strncpy_zerofill

arcade_upcall

arcade_upcall_server

arcade_upcall_server_routine

mig_impl_routine_t

mig_routine_arg_descriptor_t

mig_routine_descriptor_t

mig_routine_t

mig_stub_routine_t

