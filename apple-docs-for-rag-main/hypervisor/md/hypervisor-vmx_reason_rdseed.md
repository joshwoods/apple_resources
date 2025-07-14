

- Hypervisor
-  VMX_REASON_RDSEED 

Global Variable

# VMX_REASON_RDSEED

The guest attempted to execute RDSEED and the “RDSEED exiting” VM-execution control was 1.

macOS

``` source
var VMX_REASON_RDSEED: Int { get }
```

## See Also

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

