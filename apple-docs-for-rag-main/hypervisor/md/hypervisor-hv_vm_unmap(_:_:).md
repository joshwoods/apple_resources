

- Hypervisor
-  hv_vm_unmap(\_:\_:) 

Function

# hv_vm_unmap(\_:\_:)

Unmaps a region in the guest physical address space of the VM.

macOS 10.10+

``` source
func hv_vm_unmap(
    _ gpa: hv_gpaddr_t,
    _ size: Int
) -> hv_return_t
```

## Parameters 

`size`  

The size of the region to unmap, in bytes. It must be a multiple of the page size.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Intel-based Mac computers have different parameters:

`gpa`  
The address in the guest physical address space. It must be page-aligned.

## See Also

### Intermediate physical memory

func hv_vm_map(hv_uvaddr_t, hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Maps a region in the virtual address space of the current process into the guest physical address space of the VM.

func hv_vm_protect(hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Modifies the permissions of a region in the guest physical address space of the VM.

typealias hv_ipa_t

The type of an intermediate physical address, which is a guest physical address space of the VM.

