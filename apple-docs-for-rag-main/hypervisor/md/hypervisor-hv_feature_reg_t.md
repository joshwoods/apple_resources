

- Hypervisor
-  hv_feature_reg_t 

Structure

# hv_feature_reg_t

The type that defines feature registers.

macOS

``` source
struct hv_feature_reg_t
```

## Topics

### Feature Registers

var HV_FEATURE_REG_ID_AA64DFR0_EL1: hv_feature_reg_t

The value that identifies debug feature register 0, EL1 (DFR0_EL1).

var HV_FEATURE_REG_ID_AA64DFR1_EL1: hv_feature_reg_t

The value that identifies debug feature register 1, EL1 (DFR1_EL1).

var HV_FEATURE_REG_ID_AA64ISAR0_EL1: hv_feature_reg_t

The value that identifies instruction set attribute register 0, EL1 (ISAR0_EL1).

var HV_FEATURE_REG_ID_AA64ISAR1_EL1: hv_feature_reg_t

The value that identifies instruction set attribute register 1, EL1 (ISAR_EL1).

var HV_FEATURE_REG_ID_AA64MMFR0_EL1: hv_feature_reg_t

The value that identifies memory model feature register 0, EL1(MMFR0_EL1).

var HV_FEATURE_REG_ID_AA64MMFR1_EL1: hv_feature_reg_t

The value that identifies memory model feature register 1, EL1 (MMFR1_EL1).

var HV_FEATURE_REG_ID_AA64MMFR2_EL1: hv_feature_reg_t

The value that identifies memory model feature register 2, EL1 (MMFR2_EL1).

var HV_FEATURE_REG_ID_AA64PFR0_EL1: hv_feature_reg_t

The value that identifies processor feature register 0, EL1 (PFR0_EL1).

var HV_FEATURE_REG_ID_AA64PFR1_EL1: hv_feature_reg_t

The value that identifies processor feature register 1, EL1 (PFR1_EL1).

var HV_FEATURE_REG_CLIDR_EL1: hv_feature_reg_t

The value that describes Cache Level ID Register, EL1.

var HV_FEATURE_REG_CTR_EL0: hv_feature_reg_t

The value that describes Cache Type Register, EL0.

var HV_FEATURE_REG_DCZID_EL0: hv_feature_reg_t

The value that describes Data Cache Zero ID Register, EL0.

var HV_FEATURE_REG_ID_AA64SMFR0_EL1: hv_feature_reg_t

The value that describes Scalable Matrix Extension (SME) Feature ID Register 0.

var HV_FEATURE_REG_ID_AA64ZFR0_EL1: hv_feature_reg_t

The value that describes Scalable Vector Extension instruction (SVE) Feature ID register 0.

### Instance properties

var rawValue: UInt32

A 32-bit unsigned integer that represents the hardware feature registers.

### Initializers

init(UInt32)

Creates a new instance of the hardware feature registers.

init(rawValue: UInt32)

Creates a new instance of the hardware feature registers.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuration

func hv_vcpu_config_create() -> hv_vcpu_config_t

Creates a vCPU configuration object.

func hv_vcpu_config_get_feature_reg(hv_vcpu_config_t, hv_feature_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the value of a feature register.

func hv_vcpu_config_get_ccsidr_el1_sys_reg_values(hv_vcpu_config_t, hv_cache_type_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the Cache Size ID Register (CCSIDR_EL1) values for the vCPU configuration and cache type you specify.

typealias hv_vcpu_config_t

The type that defines a vCPU configuration.

protocol OS_hv_vcpu_config

Configuration for a virtual CPU.

