

- Hypervisor
-  VMENTRY_LOAD_IA32_PERF_GLOBAL_CTRL 

Global Variable

# VMENTRY_LOAD_IA32_PERF_GLOBAL_CTRL

The value that controls whether to load the IA32_PERF_GLOBAL_CTRL model specific register on VM entry.

macOS

``` source
var VMENTRY_LOAD_IA32_PERF_GLOBAL_CTRL: UInt32 { get }
```

## Mentioned in 

Extending vCPU Capabilities Using Model-Specific Registers

## See Also

### Capabilities

var PIN_BASED_INTR: UInt32

The value that controls whether external interrupts cause VM exits.

var PIN_BASED_NMI: UInt32

The value that controls whether external non-maskable interrupts cause VM exits.

var PIN_BASED_VIRTUAL_NMI: UInt32

The value that controls blocking of non-maskable interrupts.

var PIN_BASED_PREEMPTION_TIMER: UInt32

The value that controls whether the VMX-preemption timer counts down in VMX non-root operation.

var PIN_BASED_POSTED_INTR: UInt32

The value that controls whether the processor gives special treatment to interrupts with posted-interrupt notification vectors.

var CPU_BASED_IRQ_WND: UInt32

The value that controls whether a VM exits at the beginning of any instruction where there’s no blocking of interrupts and the interrupt flag is 1.

var CPU_BASED_TSC_OFFSET: UInt32

The value that controls whether reading the timestamp-counter MSRs changes depending on the value of the timestamp-counter offset field.

var CPU_BASED_HLT: UInt32

The value that controls whether the execution of HALT instructions cause VM exits.

var CPU_BASED_INVLPG: UInt32

The value that controls whether the execution of invalid page instructions (INVLPG) cause VM exits.

var CPU_BASED_MWAIT: UInt32

The value that controls whether the execution of Monitor Wait instructions (MWAIT) cause VM exits.

var CPU_BASED_RDPMC: UInt32

The value that controls whether the execution of Read Performance Monitoring Counters instructions (RDPMC) cause VM exits.

var CPU_BASED_RDTSC: UInt32

The value that controls whether the execution of Read Timestamp-Counter instructions (RDTSC) cause VM exits.

var CPU_BASED_CR3_LOAD: UInt32

The value that controls whether executions of MOV to Control Register 3 (CR3) cause VM exits.

var CPU_BASED_CR3_STORE: UInt32

The value that controls whether executions of MOV from Control Register 3 (CR3) cause VM exits.

var CPU_BASED_CR8_LOAD: UInt32

The value that controls whether executions of MOV to Control Register 8 (CR8) cause VM exits.

