

- Kernel
- mach
- Mach VM
-  mach_vm_read 

Function

# mach_vm_read

macOS 10.4+

``` source
kern_return_t mach_vm_read(vm_map_read_t target_task, mach_vm_address_t address, mach_vm_size_t size, vm_offset_t *data, mach_msg_type_number_t *dataCnt);
```

## See Also

### Reads and Writes

mach_vm_write

mach_vm_read_list

mach_vm_read_overwrite

