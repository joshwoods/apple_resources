

- Hypervisor
-  hv_vcpu_t 

Type Alias

# hv_vcpu_t

An opaque value that represents a vCPU instance.

macOS

``` source
typealias hv_vcpu_t = UInt64
```

## See Also

### Creation and destruction

func hv_vm_get_max_vcpu_count(UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

Returns the maximum number of vCPUs that the hypervisor supports.

func hv_vcpu_create(UnsafeMutablePointer&lt;hv_vcpuid_t>, hv_vcpu_options_t) -> hv_return_t

Creates a vCPU instance for the current thread.

func hv_vcpu_destroy(hv_vcpuid_t) -> hv_return_t

Destroys the vCPU instance associated with the current thread.

