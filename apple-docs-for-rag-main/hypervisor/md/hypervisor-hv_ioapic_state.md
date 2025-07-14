

- Hypervisor
-  hv_ioapic_state 

Structure

# hv_ioapic_state

macOS

``` source
struct hv_ioapic_state
```

## Topics

### Initializers

init()

init(rtbl: (UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64), irr: UInt32, ioa_id: UInt32, ioregsel: UInt32)

### Instance Properties

var ioa_id: UInt32

var ioregsel: UInt32

var irr: UInt32

var rtbl: (UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64, UInt64)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct hv_cache_type_t

The structure that describes an instruction or data cache element.

struct hv_vcpu_exit_exception_t

The structure that describes information about an exit from the virtual CPU (vCPU) to the host.

struct hv_apic_ctrl_t

struct hv_apic_intr_trigger_t

struct hv_apic_lvt_flavor_t

struct hv_apic_state

struct hv_apic_state_ext_t

struct hv_atpic_state

struct hv_atpic_state_ext_t

struct hv_gic_distributor_reg_t

struct hv_gic_icc_reg_t

struct hv_gic_ich_reg_t

struct hv_gic_icv_reg_t

struct hv_gic_intid_t

struct hv_gic_msi_reg_t

