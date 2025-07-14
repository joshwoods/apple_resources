

- Hypervisor
-  hv_vm_get_max_vcpu_count(\_:) 

Function

# hv_vm_get_max_vcpu_count(\_:)

Returns the maximum number of vCPUs that the hypervisor supports.

macOS 11.0+

``` source
func hv_vm_get_max_vcpu_count(_ max_vcpu_count: UnsafeMutablePointer) -> hv_return_t
```

## Parameters 

`max_vcpu_count`  

The maximum number of vCPUs on output. Undefined if the call doesn’t succeed.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## See Also

### Creation and destruction

func hv_vcpu_create(UnsafeMutablePointer&lt;hv_vcpuid_t>, hv_vcpu_options_t) -> hv_return_t

Creates a vCPU instance for the current thread.

func hv_vcpu_destroy(hv_vcpuid_t) -> hv_return_t

Destroys the vCPU instance associated with the current thread.

typealias hv_vcpu_t

An opaque value that represents a vCPU instance.

