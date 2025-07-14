

- Hypervisor
- Intel-based Mac
- Virtual Machine Control Structure (VMCS)
-  Interrupt request (IRQ) codes 

API Collection

# Interrupt request (IRQ) codes

An enumeration that describes available interrupt codes.

## Topics

### IRQ codes

var IRQ_INFO_EXT_IRQ: UInt32

The value that represents an external interrupt.

var IRQ_INFO_NMI: UInt32

The value that represents a non-maskable-interrupt.

var IRQ_INFO_HARD_EXC: UInt32

The value that represents a hardware exception.

var IRQ_INFO_SOFT_IRQ: UInt32

The value that represents a software interrupt.

var IRQ_INFO_PRIV_SOFT_EXC: UInt32

The value that represents a privileged software exception.

var IRQ_INFO_SOFT_EXC: UInt32

The value that represents a software exception interrupt.

var IRQ_INFO_ERROR_VALID: UInt32

The value that indicates the error associated with the interrupt is valid and is readable from the VMCS.

var IRQ_INFO_VALID: UInt32

The value that represents the interrupt is valid.

var IRQ_INFO_TYPE_MASK: UInt32

The value that represents the interrupt mask.

## See Also

### Shared types

VMX Creation Behavior

An enumeration that describes VMX creation behavior options.

VMX Exit Reasons

An enumertion that describes the VMX exit reasons.

