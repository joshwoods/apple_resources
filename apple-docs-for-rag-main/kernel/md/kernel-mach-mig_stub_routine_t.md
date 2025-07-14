

- Kernel
- mach
-  mig_stub_routine_t 

Type Alias

# mig_stub_routine_t

macOS 10.0+

``` source
typedef void (*mig_stub_routine_t)(mach_msg_header_t *InHeadP, mach_msg_header_t *OutHeadP);
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

mig_server_routine_t

