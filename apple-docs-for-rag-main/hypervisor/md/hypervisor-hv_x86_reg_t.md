

- Hypervisor
-  hv_x86_reg_t 

Structure

# hv_x86_reg_t

The type that defines x86 architectural registers.

macOS

``` source
struct hv_x86_reg_t
```

## Topics

### Registers

var HV_X86_RIP: hv_x86_reg_t

The value that identifies the x86 instruction pointer register.

var HV_X86_RFLAGS: hv_x86_reg_t

The value that identifies the x86 status register.

var HV_X86_RAX: hv_x86_reg_t

The value that identifies the x86 accumulator register.

var HV_X86_RCX: hv_x86_reg_t

The value that identifies the x86 counter register.

var HV_X86_RDX: hv_x86_reg_t

The value that identifies the x86 data register.

var HV_X86_RBX: hv_x86_reg_t

The value that identifies the x86 base register.

var HV_X86_RSI: hv_x86_reg_t

The value that identifies the x86 source index register.

var HV_X86_RDI: hv_x86_reg_t

The value that identifies the x86 destination index register.

var HV_X86_RSP: hv_x86_reg_t

The value that identifies the x86 stack pointer register.

var HV_X86_RBP: hv_x86_reg_t

The value that identifies the x86 base pointer register.

var HV_X86_R8: hv_x86_reg_t

The value that identifies the x86 general-purpose register R8.

var HV_X86_R9: hv_x86_reg_t

The value that identifies the x86 general-purpose register R9.

var HV_X86_R10: hv_x86_reg_t

The value that identifies the x86 general-purpose register R10.

var HV_X86_R11: hv_x86_reg_t

The value that identifies the x86 general-purpose register R11.

var HV_X86_R12: hv_x86_reg_t

The value that identifies the x86 general-purpose register R12.

var HV_X86_R13: hv_x86_reg_t

The value that identifies the x86 general-purpose register R13.

var HV_X86_R14: hv_x86_reg_t

The value that identifies the x86 general-purpose register R14.

var HV_X86_R15: hv_x86_reg_t

The value that identifies the x86 general-purpose register R15.

var HV_X86_CS: hv_x86_reg_t

The value that identifies the x86 code-segment register.

var HV_X86_SS: hv_x86_reg_t

The value that identifies the x86 stack-segment register.

var HV_X86_DS: hv_x86_reg_t

The value that identifies the x86 data-segment register.

var HV_X86_ES: hv_x86_reg_t

The value that identifies the x86 segment register ES.

var HV_X86_FS: hv_x86_reg_t

The value that identifies the x86 segment register FS.

var HV_X86_GS: hv_x86_reg_t

The value that identifies the x86 segment register GS.

var HV_X86_IDT_BASE: hv_x86_reg_t

The value that identifies the x86 interrupt descriptor, table-base register.

var HV_X86_IDT_LIMIT: hv_x86_reg_t

The value that identifies the x86 interrupt descriptor, table-base register.

var HV_X86_GDT_BASE: hv_x86_reg_t

The value that identifies the x86 global descriptor, table-base register.

var HV_X86_GDT_LIMIT: hv_x86_reg_t

The value that identifies the x86 global descriptor, table-limit register.

var HV_X86_LDTR: hv_x86_reg_t

The value that identifies the x86 local descriptor, table register.

var HV_X86_LDT_BASE: hv_x86_reg_t

The value that identifies the x86 local descriptor, table-base register.

var HV_X86_LDT_LIMIT: hv_x86_reg_t

The value that identifies the x86 local descriptor, table-limit register.

var HV_X86_LDT_AR: hv_x86_reg_t

The value that identifies the x86 local descriptor table, access-rights register.

var HV_X86_TR: hv_x86_reg_t

The value that identifies the x86 task register.

var HV_X86_TSS_BASE: hv_x86_reg_t

The value that identifies the x86 task-state, segment-base register.

var HV_X86_TSS_LIMIT: hv_x86_reg_t

The value that identifies the x86 task state segment limit register.

var HV_X86_TSS_AR: hv_x86_reg_t

The value that identifies the x86 task-state, segment-access, rights register.

var HV_X86_CR0: hv_x86_reg_t

The value that identifies the x86 control-register CR0.

var HV_X86_CR1: hv_x86_reg_t

The value that identifies the x86 control-register CR1.

var HV_X86_CR2: hv_x86_reg_t

The value that identifies the x86 control-register CR2.

var HV_X86_CR3: hv_x86_reg_t

The value that identifies the x86 control-register CR3.

var HV_X86_CR4: hv_x86_reg_t

The value that identifies the x86 control-register CR4.

var HV_X86_DR0: hv_x86_reg_t

The value that identifies the x86 debug-register DR0.

var HV_X86_DR1: hv_x86_reg_t

The value that identifies the x86 debug-register DR1.

var HV_X86_DR2: hv_x86_reg_t

The value that identifies the x86 debug-register DR2.

var HV_X86_DR3: hv_x86_reg_t

The value that identifies the x86 debug-register DR3.

var HV_X86_DR4: hv_x86_reg_t

The value that identifies the x86 debug-register DR4.

var HV_X86_DR5: hv_x86_reg_t

The value that identifies the x86 debug-register DR5.

var HV_X86_DR6: hv_x86_reg_t

The value that identifies the x86 debug-register DR6.

var HV_X86_DR7: hv_x86_reg_t

The value that identifies the x86 debug-register DR7.

var HV_X86_TPR: hv_x86_reg_t

The value that identifies the x86 task-priority register.

var HV_X86_XCR0: hv_x86_reg_t

The value that identifies the x86 extended-control register.

var HV_X86_REGISTERS_MAX: hv_x86_reg_t

The value that identifies the maximum value of x86 register constants.

### Initializers

init(UInt32)

Creates a new x86 architectural register instance.

init(rawValue: UInt32)

Creates a new x86 architectural register instance.

### Raw Value

var rawValue: UInt32

An unsigned 32-bit integer representing the x86 architectural registers.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### CPU Registers

func hv_vcpu_read_register(hv_vcpuid_t, hv_x86_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of an architectural x86 register of a vCPU.

func hv_vcpu_write_register(hv_vcpuid_t, hv_x86_reg_t, UInt64) -> hv_return_t

Sets the value of an architectural x86 register of a vCPU.

