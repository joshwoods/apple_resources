

- Hypervisor
-  IRQ_INFO_TYPE_MASK 

Global Variable

# IRQ_INFO_TYPE_MASK

The value that represents the interrupt mask.

macOS

``` source
var IRQ_INFO_TYPE_MASK: UInt32 { get }
```

## See Also

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

