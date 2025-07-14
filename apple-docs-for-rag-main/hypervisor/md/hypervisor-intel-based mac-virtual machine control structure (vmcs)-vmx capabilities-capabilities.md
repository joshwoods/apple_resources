

- Hypervisor
- Intel-based Mac
- Virtual Machine Control Structure (VMCS)
-  VMX Capabilities 

API Collection

# VMX Capabilities

An enumeration that represents the available VMX capabilities.

## Overview

The capabilites available to the hypervisor can vary depending on the specific hardware platform or OS release. Use the hv_vmx_read_capability(_:_:) API at run time to determine the capabilities that can you can select.

The example below demonstrates the process for checking for the availability a specific capability, here checking for the avaiability of timestamp-counter scaling (TSC scaling):

```
```

## Topics

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

var CPU_BASED_CR8_STORE: UInt32

The value that controls whether executions of MOV from Control Register 8 (CR8) cause VM exits.

var CPU_BASED_TPR_SHADOW: UInt32

The value that controls enabling Task Priority Register (TPR) virtualization and other APIC-virtualization features.

var CPU_BASED_VIRTUAL_NMI_WND: UInt32

The value that controls if a VM exit occurs at the beginning of any instruction if there’s no virtual-NMI blocking.

var CPU_BASED_MOV_DR: UInt32

The value that controls whether executions of MOV to or from Debug Registers (DR) cause VM exits.

var CPU_BASED_UNCOND_IO: UInt32

The value that controls whether executions of various I/O instructions cause VM exits.

var CPU_BASED_IO_BITMAPS: UInt32

The value that controls whether to use I/O bitmaps to restrict executions of I/O instructions.

var CPU_BASED_MTF: UInt32

The value that controls enabling the monitor trap flag debugging feature.

var CPU_BASED_MSR_BITMAPS: UInt32

The value that controls use of whether Model Specific Register (MSR) bitmaps to control execution of the read-from and write-to MSR instructions.

var CPU_BASED_MONITOR: UInt32

The value that controls whether executions of the Set Up Monitor Address instruction (MONITOR) cause VM exits.

var CPU_BASED_PAUSE: UInt32

The value that controls whether executions of spin-wait loop (PAUSE) instruction causes VM exits.

var CPU_BASED_SECONDARY_CTLS: UInt32

The value that conntrols use of the secondary processor-based VM-execution controls.

var CPU_BASED2_VIRTUAL_APIC: UInt32

The value that controls whether the logical processor provides special treatment for access to the Advanced Programmable Interrupt Controller (APIC).

var CPU_BASED2_EPT: UInt32

The value that controls enabling extended page tables (EPT).

var CPU_BASED2_DESC_TABLE: UInt32

The value that controls whether executions of descriptor table instructions cause VM exits.

var CPU_BASED2_RDTSCP: UInt32

The value that controls whether any execution of read timestamp-counter and processor ID instruction (RDTSCP) causes an invalid-opcode exception.

var CPU_BASED2_X2APIC: UInt32

The value that controls the logical processor’s treatment of reading/writing of Model Specific Registers to APIC MSRs.

var CPU_BASED2_VPID: UInt32

The value that controls the association of cached translations of linear addresses with a virtual processor identifier (VPID).

var CPU_BASED2_WBINVD: UInt32

The value that controls whether executions of the Invalidate Cache with Writeback instruction (WBINVD) cause VM exits.

var CPU_BASED2_UNRESTRICTED: UInt32

The value that controls whether guest software may run in unpaged protected mode or in real address mode.

var CPU_BASED2_APIC_REG_VIRT: UInt32

This value controls whether the logical processor virtualizes certain advanced programmable interrupt controller (APIC) accesses.

var CPU_BASED2_VIRT_INTR_DELIVERY: UInt32

The value that enables evaluation and delivery of pending virtual interrupts and emulation of writes to the APIC registers that control interrupt prioritization.

var CPU_BASED2_PAUSE_LOOP: UInt32

The value that controls whether a series of executions of the PAUSE instruction can cause a VM exit.

var CPU_BASED2_RDRAND: UInt32

The value that controls whether executions of the hardware random number generator instruction (RDRAND) cause VM exits.

var CPU_BASED2_INVPCID: UInt32

The value that controls whether any execution of the Invalidate Process-Context Identifier instruction (INVPCID) causes an invalid opcode exception.

var CPU_BASED2_VMFUNC: UInt32

The value that enables use of the “Invoke VM function” (VMFUNC) instruction in VMX non-root operation.

var CPU_BASED2_VMCS_SHADOW: UInt32

The value that controls whether execution of VMREAD and VMWRITE in VMX non-root operation may access a shadow VMCS instead of causing a VM exit.

var CPU_BASED2_ENCLS_EXIT_MAP: UInt32

The value that controls whether executions of Enclave Instruction Leaf Functions (ENCLS) cause examination of the ENCLS-exiting bitmap to determine whether the instruction causes a VM exit.

var CPU_BASED2_RDSEED: UInt32

The value that controls whether executions of random number generator instructions (RDSEED) cause VM exits.

var CPU_BASED2_PML: UInt32

The value that controls whether an access to a guest-physical address that sets an extended page table (EPT) dirty bit also adds an entry to the page-modification log.

var CPU_BASED2_EPT_VE: UInt32

The value that controls whether extended page table (EPT) violations cause virtualization exceptions instead of VM exits.

var CPU_BASED2_PT_CONCEAL_VMX: UInt32

The value that controls whether the processor trace facility suppresses information that the processor was in VMX non-root operation.

var CPU_BASED2_XSAVES_XRSTORS: UInt32

The value that controls whether any execution of save or restore state instructions (XSAVES or XRSTORS) causes an invalid opcode exception.

var CPU_BASED2_EPT_MODE_BASED_EXEC: UInt32

The value that controls whether to base extended page table (EPT) execute permissions on whether access to a linear address is supervisor or user mode.

var CPU_BASED2_EPT_SUBPAGE_WRITE: UInt32

The value that controls whether extended page table (EPT) write permissions specify granularity of 128 bytes.

var CPU_BASED2_PT_GUEST_PHYSICAL: UInt32

The value that controls whether to treat all output addresses used by Intel Processor Trace as guest-physical addresses and translated using the extended page table.

var CPU_BASED2_TSC_SCALING: UInt32

The value that controls whether the execution of various read time stamp counters and read model-specific registers that read from the IA32 timestamp counter model specific register return a value modified by the TSC multiplier field.

var CPU_BASED2_USER_WAIT_PAUSE: UInt32

The value that controls whether any execution of TPAUSE, UMONITOR, or UMWAIT instrucitons generate an illegal opcode exception.

var CPU_BASED2_ENCLV_EXIT_MAP: UInt32

The value that controls whether executions of an enclave VMM function instruction (ENCLV) checks the ENCLV-exiting bitmap to determine whether the instruction causes a VM exit.

var VMX_EPT_VPID_SUPPORT_AD: UInt32

The value that controls if extended page tables (EPT) support accessed and dirty flags.

var VMX_EPT_VPID_SUPPORT_EXONLY: UInt32

The value that controls whether extended page tables (EPT) support execute-only translations.

var VMEXIT_SAVE_DBG_CONTROLS: UInt32

Thievalue that controls whether to save debug register 7 DR7 and the IA32 debug control DEBUGCTL MSR on VM exit.

var VMEXIT_HOST_IA32E: UInt32

This value controls, on processors that support Intel 64 architecture, whether a logical processor is in 64-bit mode after the next VM exit.

var VMEXIT_LOAD_IA32_PERF_GLOBAL_CTRL: UInt32

The value that controls whether to load the IA32_PERF_GLOBAL_CTRL model specific register on VM exit.

var VMEXIT_ACK_INTR: UInt32

The value that controls whether the logical processor sends an acknowledgement to the interrupt controller when the VM exits.

var VMEXIT_SAVE_IA32_PAT: UInt32

The value that controls whether to save the IA32_EFER model specific register on VM exit.

var VMEXIT_LOAD_IA32_PAT: UInt32

The value that controls whether to load the IA32_EFER mode specific register on VM exit.

var VMEXIT_SAVE_EFER: UInt32

The value that controls whether to save the IA32_EFER MSR on VM exit.

var VMEXIT_LOAD_EFER: UInt32

The value that controls whether to load the IA32_EFER MSR on VM exit.

var VMEXIT_SAVE_VMX_TIMER: UInt32

The value that controls whether to save the value of the VMX-preemption timer on VM exit.

var VMEXIT_CLEAR_IA32_BNDCFGS: UInt32

The value that controls whether to clear the IA32_BNDCFGS model specific register on VM exit.

var VMEXIT_PT_CONCEAL_VMX: UInt32

The value that controls whether the Intel Processor Trace produces a paging information packet on VM exit or a VMCS packet on SMM VM exit.

var VMEXIT_CLEAR_IA32_RTIT_CTL: UInt32

The value that controls whether to clear the IA32_RTIT_CTL model specific register (MSR) on VM exit.

var VMEXIT_LOAD_CET_STATE: UInt32

The value that controls whether to load CET-related MSRs and SPP on VM exit.

var VMENTRY_LOAD_DBG_CONTROLS: UInt32

The value that controls whetherto load Debug Register 7 and the IA32_DEBUGCTL model specific register (MSR) on VM entry.

var VMENTRY_GUEST_IA32E: UInt32

The value that controls whether the logical processor is in IA-32e mode after VM entry.

var VMENTRY_SMM: UInt32

The value that controls whether the logical processor is in system-management mode (SMM) after VM entry.

var VMENTRY_DEACTIVATE_DUAL_MONITOR: UInt32

The value that controls whether the treatment of SMIs and system-management mode (SMM) is in effect after the VM entry.

var VMENTRY_LOAD_IA32_PERF_GLOBAL_CTRL: UInt32

The value that controls whether to load the IA32_PERF_GLOBAL_CTRL model specific register on VM entry.

var VMENTRY_LOAD_IA32_PAT: UInt32

The value that controls whether to load the IA32_PAT model specific register on VM entry.

var VMENTRY_LOAD_EFER: UInt32

The value that determines whether to load the IA32_EFER model specific register on VM entry.

var VMENTRY_LOAD_IA32_BNDCFGS: UInt32

The value that controls whether to load the IA32_BNDCFGS model specific register on VM entry.

var VMENTRY_PT_CONCEAL_VMX: UInt32

The value that controls whether the Intel Processor Trace produces a paging information packet (PIP) on a VM entry or a VMCS packet on a VM entry that returns from system-management mode.

var VMENTRY_LOAD_IA32_RTIT_CTL: UInt32

The value that controls whether to clear the IA32_RTIT_CTL model specific register (MSR) on VM exit.

var VMENTRY_LOAD_CET_STATE: UInt32

The value that controls whether to load CET-related model specific registers and SPP on VM exit.

## See Also

### Capabilities

func hv_vmx_read_capability(hv_vmx_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the VMX virtualization capabilities of the host processor.

func hv_vmx_get_msr_info(hv_vmx_msr_info_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns information about guest MSR configuration.

struct hv_vmx_capability_t

The type that describes Virtual Machine Extensions (VMX) capability fields.

typealias hv_vmx_msr_info_t

The type that describes Move to Status Register (MSR) information fields.

MSR Information Fields

The type that describes Machine Specific Register (MSR) fields.

