

- Kernel
- mach
-  arcade_upcall 

Function

# arcade_upcall

macOS 10.15+

``` source
kern_return_t arcade_upcall(mach_port_t arcade_upcall, vm_offset_t path, mach_msg_type_number_t pathCnt, uint64_t offset, boolean_t *should_kill);
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

arcade_upcall_server

arcade_upcall_server_routine

mig_impl_routine_t

mig_routine_arg_descriptor_t

mig_routine_descriptor_t

mig_routine_t

mig_server_routine_t

mig_stub_routine_t

