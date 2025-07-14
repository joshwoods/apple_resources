

- Hypervisor
-  hv_vcpu_destroy(\_:) 

Function

# hv_vcpu_destroy(\_:)

Destroys the vCPU instance associated with the current thread.

macOS 10.10+

``` source
func hv_vcpu_destroy(_ vcpu: hv_vcpuid_t) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### Creation and destruction

func hv_vm_get_max_vcpu_count(UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

Returns the maximum number of vCPUs that the hypervisor supports.

func hv_vcpu_create(UnsafeMutablePointer&lt;hv_vcpuid_t>, hv_vcpu_options_t) -> hv_return_t

Creates a vCPU instance for the current thread.

typealias hv_vcpu_t

An opaque value that represents a vCPU instance.

