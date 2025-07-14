

- Hypervisor
-  hv_vm_map(\_:\_:\_:\_:) 

Function

# hv_vm_map(\_:\_:\_:\_:)

Maps a region in the virtual address space of the current process into the guest physical address space of the VM.

macOS 10.10+

``` source
func hv_vm_map(
    _ uva: hv_uvaddr_t,
    _ gpa: hv_gpaddr_t,
    _ size: Int,
    _ flags: hv_memory_flags_t
) -> hv_return_t
```

## Parameters 

`size`  

The size of the mapped region in bytes. It must be a multiple of the page size.

`flags`  

The permissions for the mapped region. For a list of valid options, see hv_memory_flags_t.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

The host memory must encompass a single VM region, typically allocated with `mmap` or mach_vm_allocate instead of `malloc`.

Intel-based Mac computers have different parameters:

`uva`  
The address in the current process. It must be page-aligned.

`gpa`  
The address in the guest physical address space. It must be page-aligned.

## See Also

### Intermediate physical memory

func hv_vm_unmap(hv_gpaddr_t, Int) -> hv_return_t

Unmaps a region in the guest physical address space of the VM.

func hv_vm_protect(hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Modifies the permissions of a region in the guest physical address space of the VM.

typealias hv_ipa_t

The type of an intermediate physical address, which is a guest physical address space of the VM.

