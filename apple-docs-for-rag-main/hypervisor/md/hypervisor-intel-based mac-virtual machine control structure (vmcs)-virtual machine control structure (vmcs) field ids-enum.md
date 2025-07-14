

- Hypervisor
- Intel-based Mac
- Virtual Machine Control Structure (VMCS)
-  Virtual Machine control structure (VMCS) Field IDs 

API Collection

# Virtual Machine control structure (VMCS) Field IDs

Identify the fields of the virtual machine control structure.

## Overview

Used by the functions hv_vmx_vcpu_read_vmcs(_:_:_:) and hv_vmx_vcpu_write_vmcs(_:_:_:). The VMCS fields are read-only or read-write by the Hypervisor framework, according to the following table:

Readable and Writable VMCS Fields - Guest Fields

| Guest                    | Field                                          |
|--------------------------|------------------------------------------------|
| RIP, RSP, RFLAGS         |                                                |
| CR3, CR4, DR7            |                                                |
| Selector                 | {ES, CS, SS, DS, FS, GS, LDTR, TR}             |
| Base                     | {ES, CS, SS, DS, FS, GS, LDTR, TR, GDTR, IDTR} |
| Limit                    | {ES, CS, SS, DS, FS, GS, LDTR, TR, GDTR, IDTR} |
| Access Rights            | {ES, CS, SS, DS, FS, GS, LDTR, TR}             |
| PDPTE                    | {0, 1, 2, 3}                                   |
| CR3-Target               | {0, 1, 2, 3}                                   |
| IA32_SYSENTER_CS         |                                                |
| IA32_SYSENTER_ESP        |                                                |
| IA32_SYSENTER_EIP        |                                                |
| IA32_EFER                |                                                |
| Interruptibility State   |                                                |
| Pending Debug Exceptions |                                                |

Readable and Writable VMCS Fields - Control Fields

| Control Field                           |
|-----------------------------------------|
| Exception Bitmap                        |
| Page-Fault Error-Code Mask              |
| VM-Entry Interruption-Information Field |
| VM-Entry Exception Error Code           |
| VM-Entry Instruction Length             |
| TPR Threshold                           |
| PLE Gap                                 |
| PLE Window                              |
| CR0 Guest/Host Mask                     |
| CR4 Guest/Host Mask                     |
| CR0 Read Shadow                         |
| CR4 Read Shadow                         |

Readable and Conditionally Writable VMCS Fields - Guest Fields

| Guest Field    | Condition                   |
|----------------|-----------------------------|
| CR0            | CR0.CD and CR0.NW are unset |
| Activity State | ACTIVE or HLT               |

Readable and Conditionally Writable VMCS Fields - Control Fields

| Control Field | Condition |
|----|----|
| CR0 Guest/Host Mask | CR0.CD and CR0.NW are set |
| Pin-Based VM-Execution Controls | hv_vmx_read_capability(_:_:) returns true |
| Primary Processor-Based VM-ExecutionControls | hv_vmx_read_capability(_:_:) returns true |
| Secondary Processor-Based VM-ExecutionControls | hv_vmx_read_capability(_:_:) returns true |
| VM-Entry Controls | hv_vmx_read_capability(_:_:) returns true |

Read-Only VMCS Fields - Control Fields

| Control Field       |
|---------------------|
| TSC Offset          |
| APIC-Access Address |

Read-Only VMCS Fields - Data Fields

| Data Fields                      |
|----------------------------------|
| VM-Instruction Error             |
| Exit Reason                      |
| VM-Exit Interruption Information |
| VM-Exit Interruption Error Code  |
| IDT-Vectoring Information Field  |
| IDT-Vectoring Error Code         |
| VM-Exit Instruction Length       |
| VM-Exit Instruction Information  |
| Guest-Physical Address           |
| Exit Qualification               |
| Guest-Linear Address             |

## Topics

### IDs

var VMCS_VPID: Int

var VMCS_CTRL_POSTED_INT_N_VECTOR: Int

var VMCS_CTRL_EPTP_INDEX: Int

var VMCS_GUEST_ES: Int

var VMCS_GUEST_CS: Int

var VMCS_GUEST_SS: Int

var VMCS_GUEST_DS: Int

var VMCS_GUEST_FS: Int

var VMCS_GUEST_GS: Int

var VMCS_GUEST_LDTR: Int

var VMCS_GUEST_TR: Int

var VMCS_GUEST_INT_STATUS: Int

var VMCS_GUESTPML_INDEX: Int

var VMCS_HOST_ES: Int

var VMCS_HOST_CS: Int

var VMCS_HOST_SS: Int

var VMCS_HOST_DS: Int

var VMCS_HOST_FS: Int

var VMCS_HOST_GS: Int

var VMCS_HOST_TR: Int

var VMCS_CTRL_IO_BITMAP_A: Int

var VMCS_CTRL_IO_BITMAP_B: Int

var VMCS_CTRL_MSR_BITMAPS: Int

var VMCS_CTRL_VMEXIT_MSR_STORE_ADDR: Int

var VMCS_CTRL_VMEXIT_MSR_LOAD_ADDR: Int

var VMCS_CTRL_VMENTRY_MSR_LOAD_ADDR: Int

var VMCS_CTRL_EXECUTIVE_VMCS_PTR: Int

var VMCS_CTRL_PML_ADDR: Int

var VMCS_CTRL_TSC_OFFSET: Int

var VMCS_CTRL_VIRTUAL_APIC: Int

var VMCS_CTRL_APIC_ACCESS: Int

var VMCS_CTRL_POSTED_INT_DESC_ADDR: Int

var VMCS_CTRL_VMFUNC_CTRL: Int

var VMCS_CTRL_EPTP: Int

var VMCS_CTRL_EOI_EXIT_BITMAP_0: Int

var VMCS_CTRL_EOI_EXIT_BITMAP_1: Int

var VMCS_CTRL_EOI_EXIT_BITMAP_2: Int

var VMCS_CTRL_EOI_EXIT_BITMAP_3: Int

var VMCS_CTRL_EPTP_LIST_ADDR: Int

var VMCS_CTRL_VMREAD_BITMAP_ADDR: Int

var VMCS_CTRL_VMWRITE_BITMAP_ADDR: Int

var VMCS_CTRL_VIRT_EXC_INFO_ADDR: Int

var VMCS_CTRL_XSS_EXITING_BITMAP: Int

var VMCS_CTRL_ENCLS_EXITING_BITMAP: Int

var VMCS_CTRL_SPP_TABLE: Int

var VMCS_CTRL_TSC_MULTIPLIER: Int

var VMCS_GUEST_PHYSICAL_ADDRESS: Int

var VMCS_GUEST_LINK_POINTER: Int

var VMCS_GUEST_IA32_DEBUGCTL: Int

var VMCS_GUEST_IA32_PAT: Int

var VMCS_GUEST_IA32_EFER: Int

var VMCS_GUEST_IA32_PERF_GLOBAL_CTRL: Int

var VMCS_GUEST_PDPTE0: Int

var VMCS_GUEST_PDPTE1: Int

var VMCS_GUEST_PDPTE2: Int

var VMCS_GUEST_PDPTE3: Int

var VMCS_GUEST_IA32_BNDCFGS: Int

var VMCS_GUEST_IA32_RTIT_CTL: Int

var VMCS_HOST_IA32_PAT: Int

var VMCS_HOST_IA32_EFER: Int

var VMCS_HOST_IA32_PERF_GLOBAL_CTRL: Int

var VMCS_CTRL_PIN_BASED: Int

var VMCS_CTRL_CPU_BASED: Int

var VMCS_CTRL_EXC_BITMAP: Int

var VMCS_CTRL_PF_ERROR_MASK: Int

var VMCS_CTRL_PF_ERROR_MATCH: Int

var VMCS_CTRL_CR3_COUNT: Int

var VMCS_CTRL_VMEXIT_CONTROLS: Int

var VMCS_CTRL_VMEXIT_MSR_STORE_COUNT: Int

var VMCS_CTRL_VMEXIT_MSR_LOAD_COUNT: Int

var VMCS_CTRL_VMENTRY_CONTROLS: Int

var VMCS_CTRL_VMENTRY_MSR_LOAD_COUNT: Int

var VMCS_CTRL_VMENTRY_IRQ_INFO: Int

var VMCS_CTRL_VMENTRY_EXC_ERROR: Int

var VMCS_CTRL_VMENTRY_INSTR_LEN: Int

var VMCS_CTRL_TPR_THRESHOLD: Int

var VMCS_CTRL_CPU_BASED2: Int

var VMCS_CTRL_PLE_GAP: Int

var VMCS_CTRL_PLE_WINDOW: Int

var VMCS_RO_INSTR_ERROR: Int

var VMCS_RO_EXIT_REASON: Int

var VMCS_RO_VMEXIT_IRQ_INFO: Int

var VMCS_RO_VMEXIT_IRQ_ERROR: Int

var VMCS_RO_IDT_VECTOR_INFO: Int

var VMCS_RO_IDT_VECTOR_ERROR: Int

var VMCS_RO_VMEXIT_INSTR_LEN: Int

var VMCS_RO_VMX_INSTR_INFO: Int

var VMCS_GUEST_ES_LIMIT: Int

var VMCS_GUEST_CS_LIMIT: Int

var VMCS_GUEST_SS_LIMIT: Int

var VMCS_GUEST_DS_LIMIT: Int

var VMCS_GUEST_FS_LIMIT: Int

var VMCS_GUEST_GS_LIMIT: Int

var VMCS_GUEST_LDTR_LIMIT: Int

var VMCS_GUEST_TR_LIMIT: Int

var VMCS_GUEST_GDTR_LIMIT: Int

var VMCS_GUEST_IDTR_LIMIT: Int

var VMCS_GUEST_ES_AR: Int

var VMCS_GUEST_CS_AR: Int

var VMCS_GUEST_SS_AR: Int

var VMCS_GUEST_DS_AR: Int

var VMCS_GUEST_FS_AR: Int

var VMCS_GUEST_GS_AR: Int

var VMCS_GUEST_LDTR_AR: Int

var VMCS_GUEST_TR_AR: Int

var VMCS_GUEST_INTERRUPTIBILITY: Int

var VMCS_GUEST_IGNORE_IRQ: Int

var VMCS_GUEST_ACTIVITY_STATE: Int

var VMCS_GUEST_SMBASE: Int

var VMCS_GUEST_IA32_SYSENTER_CS: Int

var VMCS_GUEST_VMX_TIMER_VALUE: Int

var VMCS_HOST_IA32_SYSENTER_CS: Int

var VMCS_CTRL_CR0_MASK: Int

var VMCS_CTRL_CR4_MASK: Int

var VMCS_CTRL_CR0_SHADOW: Int

var VMCS_CTRL_CR4_SHADOW: Int

var VMCS_CTRL_CR3_VALUE0: Int

var VMCS_CTRL_CR3_VALUE1: Int

var VMCS_CTRL_CR3_VALUE2: Int

var VMCS_CTRL_CR3_VALUE3: Int

var VMCS_RO_EXIT_QUALIFIC: Int

var VMCS_RO_IO_RCX: Int

var VMCS_RO_IO_RSI: Int

var VMCS_RO_IO_RDI: Int

var VMCS_RO_IO_RIP: Int

var VMCS_RO_GUEST_LIN_ADDR: Int

var VMCS_GUEST_CR0: Int

var VMCS_GUEST_CR3: Int

var VMCS_GUEST_CR4: Int

var VMCS_GUEST_ES_BASE: Int

var VMCS_GUEST_CS_BASE: Int

var VMCS_GUEST_SS_BASE: Int

var VMCS_GUEST_DS_BASE: Int

var VMCS_GUEST_FS_BASE: Int

var VMCS_GUEST_GS_BASE: Int

var VMCS_GUEST_IDTR_BASE: Int

var VMCS_GUEST_TR_BASE: Int

var VMCS_GUEST_GDTR_BASE: Int

var VMCS_GUEST_LDTR_BASE: Int

var VMCS_GUEST_DR7: Int

var VMCS_GUEST_RSP: Int

var VMCS_GUEST_RIP: Int

var VMCS_GUEST_RFLAGS: Int

var VMCS_GUEST_DEBUG_EXC: Int

var VMCS_GUEST_SYSENTER_ESP: Int

var VMCS_GUEST_SYSENTER_EIP: Int

var VMCS_HOST_CR0: Int

var VMCS_HOST_CR3: Int

var VMCS_HOST_CR4: Int

var VMCS_HOST_FS_BASE: Int

var VMCS_HOST_GS_BASE: Int

var VMCS_HOST_TR_BASE: Int

var VMCS_HOST_GDTR_BASE: Int

var VMCS_HOST_IDTR_BASE: Int

var VMCS_HOST_IA32_SYSENTER_ESP: Int

var VMCS_HOST_IA32_SYSENTER_EIP: Int

var VMCS_HOST_RSP: Int

var VMCS_HOST_RIP: Int

var VMCS_MAX: Int

### Interruptibility options

var GUEST_INTRBILITY_MOVSS_BLOCKING: UInt64

var GUEST_INTRBILITY_NMI_BLOCKING: UInt64

var GUEST_INTRBILITY_SMI_BLOCKING: UInt64

var GUEST_INTRBILITY_STI_BLOCKING: UInt64

### Constants

var VMCS_INVALID: Int

var VMCS_CTRL_ENCLV_EXITING_BITMAP: Int

var VMCS_GUEST_IA32_INTR_SSP_TABLE_ADDR: Int

var VMCS_GUEST_IA32_PKRS: Int

var VMCS_GUEST_IA32_S_CET: Int

var VMCS_GUEST_SSP: Int

var VMCS_HOST_IA32_INTR_SSP_TABLE_ADDR: Int

var VMCS_HOST_IA32_PKRS: Int

var VMCS_HOST_IA32_S_CET: Int

var VMCS_HOST_SSP: Int

## See Also

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

