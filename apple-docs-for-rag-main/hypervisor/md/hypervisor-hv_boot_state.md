

- Hypervisor
-  hv_boot_state 

Enumeration

# hv_boot_state

macOS

``` source
@frozen
enum hv_boot_state
```

## Topics

### Enumeration Cases

case HV_BS_INIT

case HV_BS_RUNNING

case HV_BS_SIPI

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

VM Creation Options

Constants that describe the creation options for a virtual machine.

VM Capabilities

An enumeration that describes the capabilities of the system.

struct hv_cache_type_t

The structure that describes an instruction or data cache element.

struct hv_apic_ctrl_t

struct hv_apic_intr_trigger_t

struct hv_apic_lvt_flavor_t

struct hv_gic_distributor_reg_t

struct hv_gic_icc_reg_t

struct hv_gic_ich_reg_t

struct hv_gic_icv_reg_t

struct hv_gic_intid_t

struct hv_gic_msi_reg_t

struct hv_gic_redistributor_reg_t

struct hv_sme_p_reg_t

struct hv_sme_z_reg_t

