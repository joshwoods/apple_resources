

- Kernel
- mach
- vm
-  vm_copy 

Function

# vm_copy

macOS 10.0+

``` source
kern_return_t vm_copy(vm_map_t target_task, vm_address_t source_address, vm_size_t size, vm_address_t dest_address);
```

## See Also

### Creation and Destruction

vm_allocate

vm_allocate_cpm

vm_deallocate

mach_vm_copy

