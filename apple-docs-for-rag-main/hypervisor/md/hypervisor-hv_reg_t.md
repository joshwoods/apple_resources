

- Hypervisor
-  hv_reg_t 

Structure

# hv_reg_t

The type that defines general registers.

macOS

``` source
struct hv_reg_t
```

## Topics

### General registers

var HV_REG_CPSR: hv_reg_t

The value that identifies the current program status register (CPSR).

var HV_REG_LR: hv_reg_t

The value that identifies the link register (LR).

var HV_REG_PC: hv_reg_t

The value that identifies the program counter (PC).

var HV_REG_FP: hv_reg_t

The value that identifies the frame pointer (FP).

var HV_REG_FPCR: hv_reg_t

The value that identifies the floating-point control register (FPCR).

var HV_REG_FPSR: hv_reg_t

The value that identifies the floating-point status register (FPSR).

var HV_REG_X0: hv_reg_t

The value that identifies register X0.

var HV_REG_X1: hv_reg_t

The value that identifies register X1.

var HV_REG_X2: hv_reg_t

The value that identifies register X2.

var HV_REG_X3: hv_reg_t

The value that identifies register X3.

var HV_REG_X4: hv_reg_t

The value that identifies register X4.

var HV_REG_X5: hv_reg_t

The value that identifies register X5.

var HV_REG_X6: hv_reg_t

The value that identifies register X6.

var HV_REG_X7: hv_reg_t

The value that identifies register X7.

var HV_REG_X8: hv_reg_t

The value that identifies register X8.

var HV_REG_X9: hv_reg_t

The value that identifies register X9.

var HV_REG_X10: hv_reg_t

The value that identifies register X10.

var HV_REG_X11: hv_reg_t

The value that identifies register X11.

var HV_REG_X12: hv_reg_t

The value that identifies register X12.

var HV_REG_X13: hv_reg_t

The value that identifies register X13.

var HV_REG_X14: hv_reg_t

The value that identifies register X14.

var HV_REG_X15: hv_reg_t

The value that identifies register X15.

var HV_REG_X16: hv_reg_t

The value that identifies register X16.

var HV_REG_X17: hv_reg_t

The value that identifies register X17.

var HV_REG_X18: hv_reg_t

The value that identifies register X18.

var HV_REG_X19: hv_reg_t

The value that identifies register X19.

var HV_REG_X20: hv_reg_t

The value that identifies register X20.

var HV_REG_X21: hv_reg_t

The value that identifies register X21.

var HV_REG_X22: hv_reg_t

The value that identifies register X22.

var HV_REG_X23: hv_reg_t

The value that identifies register X23.

var HV_REG_X24: hv_reg_t

The value that identifies register X24.

var HV_REG_X25: hv_reg_t

The value that identifies register X25.

var HV_REG_X26: hv_reg_t

The value that identifies register X26.

var HV_REG_X27: hv_reg_t

The value that identifies register X27.

var HV_REG_X28: hv_reg_t

The value that identifies register X28.

var HV_REG_X29: hv_reg_t

The value that identifies register X29.

var HV_REG_X30: hv_reg_t

The value that identifies register X30.

### Instance properties

var rawValue: UInt32

A 32-bit unsigned integer that represents the general registers.

### Initializers

init(UInt32)

Creates a new general register instance initialized with the value you provide.

init(rawValue: UInt32)

Creates a new general register instance initialized with the value you provide.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### General registers

func hv_vcpu_get_reg(hv_vcpu_t, hv_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the current value of a vCPU register.

func hv_vcpu_set_reg(hv_vcpu_t, hv_reg_t, UInt64) -> hv_return_t

Sets the value of a vCPU register.

