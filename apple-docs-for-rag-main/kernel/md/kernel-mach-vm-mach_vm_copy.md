

- Kernel
- mach
- vm
-  mach_vm_copy 

Function

# mach_vm_copy

macOS 10.4+

``` source
kern_return_t mach_vm_copy(vm_map_t target_task, mach_vm_address_t source_address, mach_vm_size_t size, mach_vm_address_t dest_address);
```

## See Also

### Creation and Destruction

vm_allocate

vm_allocate_cpm

vm_deallocate

vm_copy

