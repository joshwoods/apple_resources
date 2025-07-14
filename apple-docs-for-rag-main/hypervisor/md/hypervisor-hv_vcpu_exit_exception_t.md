

- Hypervisor
-  hv_vcpu_exit_exception_t 

Structure

# hv_vcpu_exit_exception_t

The structure that describes information about an exit from the virtual CPU (vCPU) to the host.

macOS

``` source
struct hv_vcpu_exit_exception_t
```

## Topics

### Initializers

init()

Creates a new VCPU exit exception instance.

init(syndrome: hv_exception_syndrome_t, virtual_address: hv_exception_address_t, physical_address: hv_ipa_t)

Creates a new VCPU exit exception instance.with the parameters you provide.

### Instance Properties

var physical_address: hv_ipa_t

The intermediate physical address of the exception in the client.

var syndrome: hv_exception_syndrome_t

The vCPU exception syndrome causing the exception.

var virtual_address: hv_exception_address_t

The vCPU virtual address of the exception.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct hv_cache_type_t

The structure that describes an instruction or data cache element.

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

struct hv_gic_redistributor_reg_t

