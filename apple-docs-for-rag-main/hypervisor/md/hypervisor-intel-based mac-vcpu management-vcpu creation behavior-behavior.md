

- Hypervisor
- Intel-based Mac
- vCPU Management
-  vCPU Creation Behavior 

API Collection

# vCPU Creation Behavior

An enumeration representing the default creation options for virtual CPUs.

## Topics

### Constants

var HV_VCPU_DEFAULT: Int

The default vCPU creation behavior.

var HV_VCPU_ACCEL_RDPMC: Int

Instructs the kernel, when set, to handle RDPMC VM exits directly rather than passing them to user space.

var HV_VCPU_TSC_RELATIVE: Int

The value that represents the relative offset the system should add to the hypervisor TSC clock.

## See Also

### Creation and destruction

func hv_vcpu_create(UnsafeMutablePointer&lt;hv_vcpuid_t>, hv_vcpu_options_t) -> hv_return_t

Creates a vCPU instance for the current thread.

func hv_vcpu_destroy(hv_vcpuid_t) -> hv_return_t

Destroys the vCPU instance associated with the current thread.

typealias hv_vcpu_options_t

Options for creating a new vCPU instance.

typealias hv_vcpuid_t

The type that describes a vCPU ID.

