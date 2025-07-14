

- Hypervisor
-  hv_vcpu_create(\_:\_:) 

Function

# hv_vcpu_create(\_:\_:)

Creates a vCPU instance for the current thread.

macOS 10.10+

``` source
func hv_vcpu_create(
    _ vcpu: UnsafeMutablePointer,
    _ flags: hv_vcpu_options_t
) -> hv_return_t
```

## Parameters 

`vcpu`  

An argument that the hypervisor populates with the instance of a vCPU on a successful return.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Intel-based Mac computers have different parameters:

- `flags`: The vCPU creation flag. The available flags are HV_VCPU_ACCEL_RDPMC, HV_VCPU_TSC_RELATIVE, and HV_VCPU_DEFAULT. The default is HV_VCPU_DEFAULT.

Note

Using the HV_VCPU_TSC_RELATIVE flag enables use of the Time-Stamp Counter (TSC) relative offset capabilities, but disables the default TSC for vCPUs that you create with this flag.

## See Also

### Creation and destruction

func hv_vm_get_max_vcpu_count(UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

Returns the maximum number of vCPUs that the hypervisor supports.

func hv_vcpu_destroy(hv_vcpuid_t) -> hv_return_t

Destroys the vCPU instance associated with the current thread.

typealias hv_vcpu_t

An opaque value that represents a vCPU instance.

