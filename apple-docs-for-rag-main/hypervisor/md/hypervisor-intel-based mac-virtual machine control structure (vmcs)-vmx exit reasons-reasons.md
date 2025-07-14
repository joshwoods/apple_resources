

- Hypervisor
- Intel-based Mac
- Virtual Machine Control Structure (VMCS)
-  VMX Exit Reasons 

API Collection

# VMX Exit Reasons

An enumertion that describes the VMX exit reasons.

## Topics

### Exit reasons

var VMX_REASON_EXC_NMI: Int

VMX exit due to an exception or non-maskable interrupt (NMI).

var VMX_REASON_IRQ: Int

An external interrupt arrived and the “external-interrupt exiting” VM-execution control was 1.

var VMX_REASON_TRIPLE_FAULT: Int

VMX exit due to a triple fault.

var VMX_REASON_INIT: Int

VMX exit due to an INIT signal.

var VMX_REASON_SIPI: Int

VMS exit due to startup (IPI).

var VMX_REASON_IO_SMI: Int

VMX exited due to an I/O SMM Interrupt.

var VMX_REASON_OTHER_SMI: Int

An SMI arrived and caused an SMM VM exit.

var VMX_REASON_IRQ_WND: Int

VMX exited due to an Interrupt Window.

var VMX_REASON_VIRTUAL_NMI_WND: Int

At the beginning of an instruction, there was no virtual-NMI blocking.

var VMX_REASON_TASK: Int

The guest attempted a task switch.

var VMX_REASON_CPUID: Int

The guest software attempted to execute the CPUID instruction.

var VMX_REASON_GETSEC: Int

The guest attempted to execute GETSEC instruction.

var VMX_REASON_HLT: Int

The guest attempted to execute HLT and the “HLT exiting” VM-execution control was 1.

var VMX_REASON_INVD: Int

The guest attempted to execute Invalidate Caches (INVD) instruction.

var VMX_REASON_INVLPG: Int

The guest attempted to execute the Invalidate TLB Entry (INVLPG) instruction and the “INVLPG exiting” VM-execution control was 1.

var VMX_REASON_RDPMC: Int

The guest attempted to execute read performance monitoring counters (RDPMC) instruction and the “RDPMC exiting” VM-execution control was 1.

var VMX_REASON_RDTSC: Int

The guest attempted to execute read time stamp counter (RDTSC) instruction and the “RDTSC exiting” VM-execution control was 1.

var VMX_REASON_RSM: Int

The guest software attempted to execute a return from system management mode (RSM) instuction in system-management mode.

var VMX_REASON_VMCALL: Int

The execution of VMCALL by either by the guest or the executive monitor casued an ordinary VM exit or an SMM VM exit, respectively.

var VMX_REASON_VMCLEAR: Int

The guest attempted to execute VMCLEAR.

var VMX_REASON_VMLAUNCH: Int

The guest attempted to execute VMLAUNCH.

var VMX_REASON_VMPTRLD: Int

The guest attempted to execute VMPTRLD.

var VMX_REASON_VMPTRST: Int

The guest attempted to execute VMPTRST.

var VMX_REASON_VMREAD: Int

The guest attempted to execute VMREAD.

var VMX_REASON_VMRESUME: Int

The guest attempted to execute VMRESUME.

var VMX_REASON_VMWRITE: Int

The guest attempted to execute VMWRITE.

var VMX_REASON_VMOFF: Int

The guest attempted to execute VMXOFF.

var VMX_REASON_VMON: Int

The guest attempted to execute VMXON.

var VMX_REASON_MOV_CR: Int

The guest attempted to access one of the CR0, CR3, CR4 or CR8 control registers.

var VMX_REASON_MOV_DR: Int

The guest attempted a MOV to or from a debug register and the “MOV-DR exiting” VM-execution control was 1.

var VMX_REASON_IO: Int

Guest attempted to execute an I/O instruction.

var VMX_REASON_RDMSR: Int

The guest attempted to execute RDMSR.

var VMX_REASON_WRMSR: Int

The guest attempted to execute WRMSR.

var VMX_REASON_VMENTRY_GUEST: Int

VM entry failed one of the entry checks.

var VMX_REASON_VMENTRY_MSR: Int

A VM entry failed in an attempt to load model specific registers.

var VMX_REASON_MWAIT: Int

The guest attempted to execute an MWAIT instruction and the “MWAIT exiting” VM-execution control was 1.

var VMX_REASON_MTF: Int

VM exit occurred due to the setting of the monitor trap flag (MTF) or injection of a pending MTF VM exit.

var VMX_REASON_MONITOR: Int

The guest attempted to execute MONITOR and the “MONITOR exiting” VM-execution control was 1.

var VMX_REASON_PAUSE: Int

The guest attempted to execute PAUSE when the VM-execution control was 1 or exceeded the execition time window.

var VMX_REASON_VMENTRY_MC: Int

A machine-check event occurred during VM entry.

var VMX_REASON_TPR_THRESHOLD: Int

The logical processor determined that the value of the byte at offset 080H on the virtual-APIC page was below the required TPR threshold.

var VMX_REASON_APIC_ACCESS: Int

The guest attempted to access memory at a physical address on the APIC-access page and the “virtualize APIC accesses” VM-execution control was 1.

var VMX_REASON_VIRTUALIZED_EOI: Int

The system performed EOI virtualization for a virtual interrupt whose vector indexed a bit set in the EOIexit bitmap.

var VMX_REASON_GDTR_IDTR: Int

The guest attempted to execute LGDT, LIDT, SGDT, or SIDT instructions and the “descriptor-table exiting” VM-execution control was 1.

var VMX_REASON_LDTR_TR: Int

The guest attempted to execute LLDT, LTR, SLDT, or STR instructions and the “descriptor-table exiting” VM-execution control was 1.

var VMX_REASON_EPT_VIOLATION: Int

The configuration of the Extended Page Table (EPT) paging structures disallowed an attempt to access memory with a guest-physical address.

var VMX_REASON_EPT_MISCONFIG: Int

An attempt to access memory with a guest-physical address encountered a misconfigured Extended Page Table (EPT) paging-structure entry.

var VMX_REASON_EPT_INVEPT: Int

The guest attempted to execute the Invalidate cached Extended Page Table (INVEPT) instruction.

var VMX_REASON_RDTSCP: Int

The guest attempted to execute an RDTSCP instruction and the “enable RDTSCP” and “RDTSC exiting” VM-execution controls were both 1.

var VMX_REASON_VMX_TIMER_EXPIRED: Int

The preemption timer counted down to zero.

var VMX_REASON_INVVPID: Int

The guest attempted to execute the INVVPID instruction.

var VMX_REASON_WBINVD: Int

The guest attempted to execute WBINVD and the “WBINVD exiting” VM-execution control was 1.

var VMX_REASON_XSETBV: Int

The guest attempted to execute XSETBV.

var VMX_REASON_APIC_WRITE: Int

The guest completed a write to the virtual-APIC page that requires virtualization by VMM software.

var VMX_REASON_RDRAND: Int

The guest software attempted to execute RDRAND instruction and the “RDRAND exiting” VM-execution control was 1.

var VMX_REASON_INVPCID: Int

The guest attempted to execute an INVPCID instruction and the “enable INVPCID” and “INVLPG exiting” VM-execution controls were both 1.

var VMX_REASON_VMFUNC: Int

The guest called a VM function and the VM function either wasn’t enabled or generated a function-specific condition causing a VM exit.

var VMX_REASON_ENCLS: Int

The guest attempted to execute an unsupported ENCLS instruction.

var VMX_REASON_RDSEED: Int

The guest attempted to execute RDSEED and the “RDSEED exiting” VM-execution control was 1.

var VMX_REASON_PML_FULL: Int

var VMX_REASON_XSAVES: Int

The guest attempted to execute XSAVES which wasn’t allowed in the current configuration.

var VMX_REASON_XRSTORS: Int

The guest attempted to execute XRSTORS which wasn’t allowed in the current configuration.

var VMX_REASON_SPP_EVENT: Int

The processor attempted to determine an access’s sub-page write permission and encountered an SPP miss or an SPP misconfiguration.

var VMX_REASON_UMWAIT: Int

The guest attempted to execute a UMWAIT instruction and both the “enable user wait and pause” and “RDTSC exiting” VM-execution controls were both 1.

var VMX_REASON_TPAUSE: Int

The guest attempted to execute a TPAUSE instuction and both the “enable user wait and pause” and “RDTSC exiting” VM-execution controls were both 1.

## See Also

### Shared types

VMX Creation Behavior

An enumeration that describes VMX creation behavior options.

Interrupt request (IRQ) codes

An enumeration that describes available interrupt codes.

