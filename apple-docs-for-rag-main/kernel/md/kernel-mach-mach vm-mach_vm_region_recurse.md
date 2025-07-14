

- Kernel
- mach
- Mach VM
-  mach_vm_region_recurse 

Function

# mach_vm_region_recurse

macOS 10.4+

``` source
kern_return_t mach_vm_region_recurse(vm_map_read_t target_task, mach_vm_address_t *address, mach_vm_size_t *size, natural_t *nesting_depth, vm_region_recurse_info_t info, mach_msg_type_number_t *infoCnt);
```

## See Also

### Regions

mach_vm_region

mach_vm_region_info

mach_vm_region_info_64

