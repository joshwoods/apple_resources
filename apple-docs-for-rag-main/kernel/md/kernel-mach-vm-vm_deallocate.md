

- Kernel
- mach
- vm
-  vm_deallocate 

Function

# vm_deallocate

macOS 10.0+

``` source
kern_return_t vm_deallocate(vm_map_t target_task, vm_address_t address, vm_size_t size);
```

## See Also

### Creation and Destruction

vm_allocate

vm_allocate_cpm

vm_copy

mach_vm_copy

