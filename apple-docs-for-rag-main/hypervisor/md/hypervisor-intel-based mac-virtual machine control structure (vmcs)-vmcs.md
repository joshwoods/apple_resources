

- Hypervisor
- Intel-based Mac
-  Virtual Machine Control Structure (VMCS) 

API Collection

# Virtual Machine Control Structure (VMCS)

Read and write to fields of the virtual machine control structure.

## Topics

### Capabilities

func hv_vmx_read_capability(hv_vmx_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the VMX virtualization capabilities of the host processor.

func hv_vmx_get_msr_info(hv_vmx_msr_info_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns information about guest MSR configuration.

struct hv_vmx_capability_t

The type that describes Virtual Machine Extensions (VMX) capability fields.

VMX Capabilities

An enumeration that represents the available VMX capabilities.

typealias hv_vmx_msr_info_t

The type that describes Move to Status Register (MSR) information fields.

MSR Information Fields

The type that describes Machine Specific Register (MSR) fields.

### Field management

Virtual Machine Control Structure (VMCS) Field IDs

Fields you can read or change using the Hypervisor framework’s read and write functions.

func hv_vmx_vcpu_read_vmcs(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of a virtual machine control structure (VMCS) field of a vCPU.

func hv_vmx_vcpu_write_vmcs(hv_vcpuid_t, UInt32, UInt64) -> hv_return_t

Sets the value of a virtual machine control structure (VMCS) field of a vCPU.

func hv_vmx_vcpu_get_cap_write_vmcs(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the allowed_0 and allowed_1 masks for a VMCS field of a vCPU.

func hv_vmx_vcpu_set_apic_address(hv_vcpuid_t, hv_gpaddr_t) -> hv_return_t

Sets the address of the guest Advanced Programmable Interrupt Controller (APIC) for a vCPU in the guest physical address space of the VM.

Virtual Machine control structure (VMCS) Field IDs

Identify the fields of the virtual machine control structure.

### Shadow fields

func hv_vmx_vcpu_read_shadow_vmcs(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the current value of a shadow VMCS field of a vCPU.

func hv_vmx_vcpu_set_shadow_access(hv_vcpuid_t, UInt32, hv_shadow_flags_t) -> hv_return_t

Set the access permissions of a shadow VMCS field of a vCPU.

func hv_vmx_vcpu_write_shadow_vmcs(hv_vcpuid_t, UInt32, UInt64) -> hv_return_t

Set the value of a shadow VMCS field of a vCPU.

typealias hv_shadow_flags_t

Shadow VMCS permissions for the set shadow access function.

Shadow Permissions

Permissions that define access to the shadow VMCS fields.

### Shared types

VMX Creation Behavior

An enumeration that describes VMX creation behavior options.

VMX Exit Reasons

An enumertion that describes the VMX exit reasons.

Interrupt request (IRQ) codes

An enumeration that describes available interrupt codes.

## See Also

### Resource management

vCPU Management

Create and run virtual CPUs, and manage CPU-specific registers and features.

Memory Management

Map memory into the physical address space of the virtual machine, and allocate additional memory for the current task.

