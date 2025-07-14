

- Kernel
- mach
- Mach VM
-  mach_vm_write 

Function

# mach_vm_write

macOS 10.4+

``` source
kern_return_t mach_vm_write(vm_map_t target_task, mach_vm_address_t address, vm_offset_t data, mach_msg_type_number_t dataCnt);
```

## See Also

### Reads and Writes

mach_vm_read

mach_vm_read_list

mach_vm_read_overwrite

