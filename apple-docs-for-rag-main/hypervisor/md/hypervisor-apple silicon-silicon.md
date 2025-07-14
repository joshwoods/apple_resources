

- Hypervisor
-  Apple Silicon 

API Collection

# Apple Silicon

Create and run virtual machines on Apple silicon.

## Topics

### Virtual machine management

func hv_vm_config_create() -> hv_vm_config_t

Creates a virtual machine configuration object.

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

protocol OS_hv_vm_config

Creates a virtual machine configuration object.

typealias hv_vm_config_t

The type that defines a virtual-machine configuration.

### Resource management

vCPU Management

Create and run virtual CPUs, and manage CPU-specific registers and features.

Memory management

Map memory into the physical address space of the virtual machine.

### Timer functions

func hv_vcpu_get_vtimer_mask(hv_vcpu_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Gets the virtual timer mask.

func hv_vcpu_set_vtimer_mask(hv_vcpu_t, Bool) -> hv_return_t

Sets or clears the virtual timer mask.

func hv_vcpu_get_vtimer_offset(hv_vcpu_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the vTimer offset for the vCPU ID you specify.

func hv_vcpu_set_vtimer_offset(hv_vcpu_t, UInt64) -> hv_return_t

Sets the vTimer offset to a value that you provide.

### Common data types

typealias hv_return_t

The return type of framework functions.

Hypervisor Errors

Return codes returned by framework functions.

### Nested virtualization

func hv_vm_config_get_el2_supported(UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Returns a status value that indicates whether the current platform supports Exception Level 2 (EL2).

func hv_vm_config_get_el2_enabled(hv_vm_config_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Return a status value that indicates whether the VM configuration enables support for Exception Level 2 (EL2).

func hv_vm_config_set_el2_enabled(hv_vm_config_t, Bool) -> hv_return_t

Sets whether the specified VM configuration enables support for Exception Level 2 (EL2).

### Generic interrupt controllers (GICs)

GIC functions

These functions and registers support the creation and operation of a generic interrupt controller.

GIC registers

These registers support the operation of a generic interrupt controller and its interface with the Hypervisor and virtual CPUs.

## See Also

### Platforms

Intel-based Mac

Create and run virtual machines on Intel-based Mac computers.

