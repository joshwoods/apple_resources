

- Hypervisor
-  hv_memory_flags_t 

Type Alias

# hv_memory_flags_t

The permissions for guest physical memory regions.

macOS

``` source
typealias hv_memory_flags_t = UInt64
```

## Discussion

Set with the hv_vm_map(_:_:_:_:) and hv_vm_protect(_:_:_:) functions.

## Topics

### Permissions

var HV_MEMORY_READ: Int

The value that represents the memory-read permission.

var HV_MEMORY_WRITE: Int

The value that represents the memory-write permission.

var HV_MEMORY_EXEC: Int

The value that represents the memory-execute permission.

## See Also

### Data Types

typealias hv_allocate_flags_t

typealias hv_gpaddr_t

The type of a guest physical address (GPA).

typealias hv_sme_zt0_uchar64_t

typealias hv_uvaddr_t

The type of a user virtual address.

typealias hv_vm_space_t

The type of a guest-address space.

