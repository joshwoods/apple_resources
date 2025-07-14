

- Kernel
- Kernel Functions
-  vm_remap_new 

Function

# vm_remap_new

macOS 11.3+

``` source
kern_return_t vm_remap_new(vm_map_t target_task, vm_address_t *target_address, vm_size_t size, vm_address_t mask, int flags, vm_map_read_t src_task, vm_address_t src_address, boolean_t copy, vm_prot_t *cur_protection, vm_prot_t *max_protection, vm_inherit_t inheritance);
```

