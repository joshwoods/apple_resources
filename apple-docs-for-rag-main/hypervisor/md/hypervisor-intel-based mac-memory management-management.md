

- Hypervisor
- Intel-based Mac
-  Memory Management 

API Collection

# Memory Management

Map memory into the physical address space of the virtual machine, and allocate additional memory for the current task.

## Topics

### Shared memory

func hv_vm_map(hv_uvaddr_t, hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Maps a region in the virtual address space of the current process into the guest physical address space of the VM.

func hv_vm_unmap(hv_gpaddr_t, Int) -> hv_return_t

Unmaps a region in the guest physical address space of the VM.

func hv_vm_protect(hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Modifies the permissions of a region in the guest physical address space of the VM.

### Process-specific memory

func hv_vm_space_create(UnsafeMutablePointer&lt;hv_vm_space_t>) -> hv_return_t

Creates an additional guest address space for the current task.

func hv_vm_space_destroy(hv_vm_space_t) -> hv_return_t

Destroys the address space instance associated with the current task.

func hv_vm_map_space(hv_vm_space_t, hv_uvaddr_t, hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Maps a region in the virtual address space of the current task into a guest physical address space of the VM.

func hv_vm_unmap_space(hv_vm_space_t, hv_gpaddr_t, Int) -> hv_return_t

Umaps a region in a guest physical address space of the VM.

func hv_vm_protect_space(hv_vm_space_t, hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Modifies the permissions of a region in a guest physical address space of the VM.

### Common types

typealias hv_uvaddr_t

The type of a user virtual address.

typealias hv_gpaddr_t

The type of a guest physical address (GPA).

typealias hv_memory_flags_t

The permissions for guest physical memory regions.

Memory Permissions

Enumeration values that describe memory permissions.

typealias hv_vm_space_t

The type of a guest-address space.

Address Space Types

## See Also

### Resource management

vCPU Management

Create and run virtual CPUs, and manage CPU-specific registers and features.

Virtual Machine Control Structure (VMCS)

Read and write to fields of the virtual machine control structure.

