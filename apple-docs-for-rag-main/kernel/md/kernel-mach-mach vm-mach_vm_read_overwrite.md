

- Kernel
- mach
- Mach VM
-  mach_vm_read_overwrite 

Function

# mach_vm_read_overwrite

macOS 10.4+

``` source
kern_return_t mach_vm_read_overwrite(vm_map_read_t target_task, mach_vm_address_t address, mach_vm_size_t size, mach_vm_address_t data, mach_vm_size_t *outsize);
```

## See Also

### Reads and Writes

mach_vm_read

mach_vm_write

mach_vm_read_list

