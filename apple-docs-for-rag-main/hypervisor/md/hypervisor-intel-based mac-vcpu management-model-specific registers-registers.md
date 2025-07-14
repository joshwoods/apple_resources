

- Hypervisor
- Intel-based Mac
- vCPU Management
-  Model-Specific Registers 

API Collection

# Model-Specific Registers

## Topics

### Constants

var HV_MSR_IA32_ARCH_CAPABILITIES: UInt32

The value that represents the Model-Specific Register (MSR) that you use to enumerate processor capabilities.

var HV_MSR_IA32_A_PMC0: UInt32

The value that represents support for address performance-counter register 0.

var HV_MSR_IA32_A_PMC7: UInt32

The value that represents support for address performance-counter register 7.

var HV_MSR_IA32_CSTAR: UInt32

The value that represents the address of IA-32e Mode System Call Target Address.

var HV_MSR_IA32_DEBUGCTL: UInt32

The value that represents the address of the Debug Control Register.

var HV_MSR_IA32_EFER: UInt32

The value that represents the address of the Entended Feature Enable Register (EFER).

var HV_MSR_IA32_FIXED_CTR0: UInt32

The value that represents the address of Fixed-Function Performance Counter Register 0.

var HV_MSR_IA32_FIXED_CTR1: UInt32

The value that represents the address of Fixed-Function Performance Counter Register 1.

var HV_MSR_IA32_FIXED_CTR2: UInt32

The value that represents the address of Fixed-Function Performance Counter Register 2.

var HV_MSR_IA32_FIXED_CTR3: UInt32

The value that represents the address of Fixed-Function Performance Counter Register 3.

var HV_MSR_IA32_FIXED_CTR_CTRL: UInt32

The value that represents the address of the Fixed-Function Counter Control Register.

var HV_MSR_IA32_FLUSH_CMD: UInt32

The value that represents the address of the Flush Command Register.

var HV_MSR_IA32_FMASK: UInt32

The value that represents the address of the System Call Flag Mask (FMASK) Register.

var HV_MSR_IA32_FS_BASE: UInt32

The value that represents the address of the map for the base address of the FS segment register.

var HV_MSR_IA32_GS_BASE: UInt32

The value that represents the address of the map for the base address of the GS segment register.

var HV_MSR_IA32_KERNEL_GS_BASE: UInt32

The value that represents the address swap target for the base address of the GS segment register.

var HV_MSR_IA32_LSTAR: UInt32

The value that represents the address of the IA-32e Mode System Call Target Address.

var HV_MSR_IA32_PERFEVNTSEL0: UInt32

The value that represents the address of Performance Event Select Counter 0.

var HV_MSR_IA32_PERFEVNTSEL7: UInt32

The value that represents the address of Performance Event Select Counter 7.

var HV_MSR_IA32_PERF_GLOBAL_CTRL: UInt32

The value that represents the address of the Global Performance Counter Control Register.

var HV_MSR_IA32_PERF_GLOBAL_INUSE: UInt32

The value that represents the address of the register that indicates whether the core performance monitor interface is in use.

var HV_MSR_IA32_PERF_GLOBAL_STATUS: UInt32

The value that represents the address of the Global Performance Status Register.

var HV_MSR_IA32_PERF_GLOBAL_STATUS_RESET: UInt32

The value that represents the address of the Global Performance Counter Overflow Reset Control Register.

var HV_MSR_IA32_PERF_GLOBAL_STATUS_SET: UInt32

The value that represents the address of the Global Performance Counter Overflow Set Control Register.

var HV_MSR_IA32_PMC0: UInt32

The value that represents the address of Performance Counter Register 0.

var HV_MSR_IA32_PMC7: UInt32

The value that represents the address of Performance Counter Register 7.

var HV_MSR_IA32_PRED_CMD: UInt32

The value that represents the address of the Prediction Command Register.

var HV_MSR_IA32_SPEC_CTRL: UInt32

The value that represents the address of Speculation Control Register.

var HV_MSR_IA32_STAR: UInt32

The value that represents the address of the System Call Target Address Register.

var HV_MSR_IA32_SYSENTER_CS: UInt32

The value that represents the address of the CS Register target for Current Privilege Level (CPL) 0 code.

var HV_MSR_IA32_SYSENTER_EIP: UInt32

The value that represents the address of the Extended Instruction Pointer (EIP) Register target for Current Privilege Level (CPL) 0 code.

var HV_MSR_IA32_SYSENTER_ESP: UInt32

The value that represents the address of the Extended Stack Pointer (ESP) Register target for Current Privilege Level (CPL) 0 code.

var HV_MSR_IA32_TSC: UInt32

The value that represents the address of the Time-Stamp Counter Register.

var HV_MSR_IA32_TSC_AUX: UInt32

The value that represents the address of the Auxiliary Time-Stamp Counter Register.

var HV_MSR_IA32_XSS: UInt32

The value that represents the address of the Extended Supervisors State Mask (XSS) Register.

var HV_MSR_LASTBRANCH_0_FROM_IP: UInt32

The value that represents the address of the Last Branch Record 0 from Instruction Pointer (IP) register.

var HV_MSR_LASTBRANCH_0_TO_IP: UInt32

The value that represents the address of the Last Branch Record 0 to Instruction Pointer (IP) register.

var HV_MSR_LASTBRANCH_31_FROM_IP: UInt32

The value that represents the address of the Last Branch Record 31 from Instruction Pointer (IP) register.

var HV_MSR_LASTBRANCH_31_TO_IP: UInt32

The value that represents the address of the Last Branch Record 31 to Instruction Pointer (IP) register.

var HV_MSR_LASTBRANCH_INFO_0: UInt32

The value that represents the address of the Last Branch Record 0 additional information register.

var HV_MSR_LASTBRANCH_INFO_31: UInt32

The value that represents the address of the Last Branch Record 31 additional information register.

var HV_MSR_LASTBRANCH_TOS: UInt32

The value that represents the address of the Last Branch Record Top of Stack (TOS) Register.

var HV_MSR_LASTINT_FROM_IP: UInt32

The value that represents the address of the Last Interrupt from Instruction Pointer (IP) Register.

var HV_MSR_LASTINT_TO_IP: UInt32

The value that represents the address of the Last Interrupt to Instruction Pointer (IP) Register.

var HV_MSR_LBR_SELECT: UInt32

The value that represents the address of the Last Branch Record Filtering Select Register.

var HV_MSR_PERF_METRICS: UInt32

The value that represents the address of the Performance Metrics Register.

## See Also

### Model-Specific Registers

Extending vCPU Capabilities Using Model-Specific Registers

Configure specific client performance monitoring and enable other vCPU capabilities using Model-Specific Registers.

func hv_vcpu_read_msr(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of a Model-Specific Register (MSR) of a vCPU.

func hv_vcpu_write_msr(hv_vcpuid_t, UInt32, UInt64) -> hv_return_t

Sets the value of a Model-Specific Register (MSR) of a vCPU.

func hv_vcpu_enable_native_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables or disables a Model-Specific Register (MSR) that the VM uses natively.

func hv_vcpu_set_msr_access(hv_vcpuid_t, UInt32, hv_msr_flags_t) -> hv_return_t

Controls the guest access of a managed Model-Specific Register (MSR).

func hv_vcpu_enable_managed_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables the guest access of a managed Model-Specific Register (MSR).

typealias hv_msr_flags_t

The type representing the native Model-Specific Register (MSR) permissions.

MSR Permissions

An enumeration that describes possible Model-Specific Register (MSR) permisssions.

