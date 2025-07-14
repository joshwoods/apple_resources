

- Hypervisor
-  hv_ipa_t 

Type Alias

# hv_ipa_t

The type of an intermediate physical address, which is a guest physical address space of the VM.

macOS

``` source
typealias hv_ipa_t = UInt64
```

## See Also

### Intermediate physical memory

func hv_vm_map(hv_uvaddr_t, hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Maps a region in the virtual address space of the current process into the guest physical address space of the VM.

func hv_vm_unmap(hv_gpaddr_t, Int) -> hv_return_t

Unmaps a region in the guest physical address space of the VM.

func hv_vm_protect(hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Modifies the permissions of a region in the guest physical address space of the VM.

