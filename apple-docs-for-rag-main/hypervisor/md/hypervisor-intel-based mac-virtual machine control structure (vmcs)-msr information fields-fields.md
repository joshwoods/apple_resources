

- Hypervisor
- Intel-based Mac
- Virtual Machine Control Structure (VMCS)
-  MSR Information Fields 

API Collection

# MSR Information Fields

The type that describes Machine Specific Register (MSR) fields.

## Topics

### Fields

var HV_VMX_INFO_MSR_IA32_ARCH_CAPABILITIES: Int

The value of the IA32 architecture capabilities model specific register.

var HV_VMX_INFO_MSR_IA32_PERF_CAPABILITIES: Int

The value of the IA32 performance capabilities model specific register.

var HV_VMX_VALID_MSR_IA32_PERFEVNTSEL: Int

The bitmask of the supported fields of the IA32 Performance-Event Selection Mode model specific register.

var HV_VMX_VALID_MSR_IA32_FIXED_CTR_CTRL: Int

The bitmask fo the supported fields of the Fixed-Function-Counter Control Register.

var HV_VMX_VALID_MSR_IA32_PERF_GLOBAL_CTRL: Int

The bitmask of the supported fields of the IA32 Global-Counter Control Facility Register.

var HV_VMX_VALID_MSR_IA32_PERF_GLOBAL_STATUS: Int

The bitmast of the supported fields of the Global-Counter-Control Status model specific register.

var HV_VMX_VALID_MSR_IA32_DEBUGCTL: Int

The bitmask of the IA32 Debug-Control model specific register.

var HV_VMX_VALID_MSR_IA32_SPEC_CTRL: Int

The bitmask of the suppported fields of the Speculation Control model specific register.

var HV_VMX_NEED_MSR_IA32_SPEC_CTRL: Int

The bitmask of the required fields of the IA32 Speculation Control model specific register.

## See Also

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

