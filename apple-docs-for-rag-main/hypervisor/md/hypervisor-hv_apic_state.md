

- Hypervisor
-  hv_apic_state 

Structure

# hv_apic_state

macOS

``` source
struct hv_apic_state
```

## Topics

### Initializers

init()

init(apic_gpa: UInt64, apic_controls: UInt64, tsc_deadline: UInt64, apic_id: UInt32, ver: UInt32, tpr: UInt32, apr: UInt32, ldr: UInt32, dfr: UInt32, svr: UInt32, isr: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32), tmr: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32), irr: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32), esr: UInt32, lvt: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32), icr: (UInt32, UInt32), icr_timer: UInt32, dcr_timer: UInt32, ccr_timer: UInt32, esr_pending: UInt32, boot_state: hv_boot_state, aeoi: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32))

### Instance Properties

var aeoi: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32)

var apic_controls: UInt64

var apic_gpa: UInt64

var apic_id: UInt32

var apr: UInt32

var boot_state: hv_boot_state

var ccr_timer: UInt32

var dcr_timer: UInt32

var dfr: UInt32

var esr: UInt32

var esr_pending: UInt32

var icr: (UInt32, UInt32)

var icr_timer: UInt32

var irr: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32)

var isr: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32)

var ldr: UInt32

var lvt: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32)

var svr: UInt32

var tmr: (UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32, UInt32)

var tpr: UInt32

var tsc_deadline: UInt64

var ver: UInt32

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

struct hv_apic_state_ext_t

struct hv_atpic_state

struct hv_atpic_state_ext_t

struct hv_gic_distributor_reg_t

struct hv_gic_icc_reg_t

struct hv_gic_ich_reg_t

struct hv_gic_icv_reg_t

struct hv_gic_intid_t

struct hv_gic_msi_reg_t

struct hv_gic_redistributor_reg_t

