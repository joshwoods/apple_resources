

- Hypervisor
-  hv_atpic_state 

Structure

# hv_atpic_state

macOS

``` source
struct hv_atpic_state
```

## Topics

### Initializers

init()

init(ready: Bool, icw_num: UInt8, rd_cmd_reg: UInt8, aeoi: Bool, poll: Bool, rotate: Bool, sfn: Bool, irq_base: UInt8, request: UInt8, service: UInt8, mask: UInt8, smm: Bool, last_request: UInt8, lowprio: UInt8, intr_raised: Bool, elc: UInt8)

### Instance Properties

var aeoi: Bool

var elc: UInt8

var icw_num: UInt8

var intr_raised: Bool

var irq_base: UInt8

var last_request: UInt8

var lowprio: UInt8

var mask: UInt8

var poll: Bool

var rd_cmd_reg: UInt8

var ready: Bool

var request: UInt8

var rotate: Bool

var service: UInt8

var sfn: Bool

var smm: Bool

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

struct hv_atpic_state_ext_t

struct hv_gic_distributor_reg_t

struct hv_gic_icc_reg_t

struct hv_gic_ich_reg_t

struct hv_gic_icv_reg_t

struct hv_gic_intid_t

struct hv_gic_msi_reg_t

struct hv_gic_redistributor_reg_t

