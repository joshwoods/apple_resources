

- Kernel
- mach
- Mach VM
-  mach_vm_region_info_64 

Function

# mach_vm_region_info_64

macOS 10.0+

``` source
kern_return_t mach_vm_region_info_64(vm_map_read_t task, vm_address_t address, vm_info_region_64_t *region, vm_info_object_array_t *objects, mach_msg_type_number_t *objectsCnt);
```

## See Also

### Regions

mach_vm_region

mach_vm_region_info

mach_vm_region_recurse

