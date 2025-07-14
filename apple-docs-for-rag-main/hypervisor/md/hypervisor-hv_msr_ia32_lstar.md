

- Hypervisor
-  HV_MSR_IA32_LSTAR 

Global Variable

# HV_MSR_IA32_LSTAR

The value that represents the address of the IA-32e Mode System Call Target Address.

macOS

``` source
var HV_MSR_IA32_LSTAR: UInt32 { get }
```

## Discussion

This address is the target Instruction Pointer Register (RIP) address for the procedure SYSCALL executes in 64-bit mode.

## See Also

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

