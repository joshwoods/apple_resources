

- Hypervisor
-  hv_vmx_capability_t 

Structure

# hv_vmx_capability_t

The type that describes Virtual Machine Extensions (VMX) capability fields.

macOS

``` source
struct hv_vmx_capability_t
```

## Topics

### Capabilities

var HV_VMX_CAP_PINBASED: hv_vmx_capability_t

Field ID for pin-based capabilities.

var HV_VMX_CAP_PROCBASED: hv_vmx_capability_t

Field ID for primary proc-based capabilities.

var HV_VMX_CAP_PROCBASED2: hv_vmx_capability_t

Field ID for secondary proc-based capabilities.

var HV_VMX_CAP_ENTRY: hv_vmx_capability_t

Field ID for VM entry capabilities.

var HV_VMX_CAP_EXIT: hv_vmx_capability_t

Field ID for VM exit capabilities.

var HV_VMX_CAP_BASIC: hv_vmx_capability_t

Field ID for basic VMX capabilities.

var HV_VMX_CAP_TRUE_PINBASED: hv_vmx_capability_t

Field ID for hardware pin-based VMX capabilities.

var HV_VMX_CAP_TRUE_PROCBASED: hv_vmx_capability_t

Field ID for primary process-based VMX capabilities.

var HV_VMX_CAP_TRUE_ENTRY: hv_vmx_capability_t

Field ID for hardware VM-entry VMX capabilities.

var HV_VMX_CAP_TRUE_EXIT: hv_vmx_capability_t

Field ID for hardware VM-exit VMX capabilities.

var HV_VMX_CAP_MISC: hv_vmx_capability_t

Field ID for miscellaneous VMX capabilities.

var HV_VMX_CAP_CR0_FIXED0: hv_vmx_capability_t

Field ID for CR0 allowed, zero-bits VMX capability.

var HV_VMX_CAP_CR0_FIXED1: hv_vmx_capability_t

Field ID for CR0 allowed, one-bits VMX capability.

var HV_VMX_CAP_CR4_FIXED0: hv_vmx_capability_t

Fields ID for CR4 allowed, zero-bits VMX capability.

var HV_VMX_CAP_CR4_FIXED1: hv_vmx_capability_t

Field ID for CR4 allowed, one-bits VMX capability.

var HV_VMX_CAP_VMCS_ENUM: hv_vmx_capability_t

Field ID for VMCS enumeration capability.

var HV_VMX_CAP_EPT_VPID_CAP: hv_vmx_capability_t

Field ID for EPT/VPID VMX capabilities.

var HV_VMX_CAP_PREEMPTION_TIMER: hv_vmx_capability_t

Field ID for preemption timer frequency.

### Initializers

init(UInt32)

Creates a new Virtual Machine Extensions (VMX) instance.

init(rawValue: UInt32)

Creates a new Virtual Machine Extensions (VMX) instance with the value you provide.

### Raw Value

var rawValue: UInt32

An unsigned 32-bit integer that represents the Virtual Machine Extensions (VMX) fields.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Capabilities

func hv_vmx_read_capability(hv_vmx_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the VMX virtualization capabilities of the host processor.

func hv_vmx_get_msr_info(hv_vmx_msr_info_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns information about guest MSR configuration.

VMX Capabilities

An enumeration that represents the available VMX capabilities.

typealias hv_vmx_msr_info_t

The type that describes Move to Status Register (MSR) information fields.

MSR Information Fields

The type that describes Machine Specific Register (MSR) fields.

