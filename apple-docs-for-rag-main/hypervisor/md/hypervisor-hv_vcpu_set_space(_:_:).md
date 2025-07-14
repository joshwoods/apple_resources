

- Hypervisor
-  hv_vcpu_set_space(\_:\_:) 

Function

# hv_vcpu_set_space(\_:\_:)

Associates the vCPU instance with an allocated address space.

macOS 10.15+

``` source
func hv_vcpu_set_space(
    _ vcpu: hv_vcpuid_t,
    _ asid: hv_vm_space_t
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`asid`  

The address space ID.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

