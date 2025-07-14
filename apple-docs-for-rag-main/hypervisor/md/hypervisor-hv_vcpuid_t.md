

- Hypervisor
-  hv_vcpuid_t 

Type Alias

# hv_vcpuid_t

The type that describes a vCPU ID.

macOS

``` source
typealias hv_vcpuid_t = UInt32
```

## See Also

### Creation and destruction

func hv_vcpu_create(UnsafeMutablePointer&lt;hv_vcpuid_t>, hv_vcpu_options_t) -> hv_return_t

Creates a vCPU instance for the current thread.

func hv_vcpu_destroy(hv_vcpuid_t) -> hv_return_t

Destroys the vCPU instance associated with the current thread.

typealias hv_vcpu_options_t

Options for creating a new vCPU instance.

vCPU Creation Behavior

An enumeration representing the default creation options for virtual CPUs.

