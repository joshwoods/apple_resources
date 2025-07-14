

- Kernel
- mach
- vm
-  vm_allocate 

Function

# vm_allocate

macOS 10.0+

``` source
kern_return_t vm_allocate(vm_map_t target_task, vm_address_t *address, vm_size_t size, int flags);
```

## See Also

### Creation and Destruction

vm_allocate_cpm

vm_deallocate

vm_copy

mach_vm_copy

