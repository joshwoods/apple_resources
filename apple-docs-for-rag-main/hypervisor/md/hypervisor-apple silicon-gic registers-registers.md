

- Hypervisor
- Apple Silicon
-  GIC registers 

API Collection

# GIC registers

These registers support the operation of a generic interrupt controller and its interface with the Hypervisor and virtual CPUs.

## Discussion

For more information on the purpose of specific register sets and their operation in GICs, see the ARM Generic Interrupt Controller (GIC) v3 architecture specification.

## Topics

### Distributor registers

Distributor registers

### Redistributor registers

var HV_GIC_REDISTRIBUTOR_REG_GICR_TYPER: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ICACTIVER0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ICENABLER0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ICFGR0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ICFGR1: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ICPENDR0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IGROUPR0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR1: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR2: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR3: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR4: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR5: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR6: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_IPRIORITYR7: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ISACTIVER0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ISENABLER0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_ISPENDR0: hv_gic_redistributor_reg_t

var HV_GIC_REDISTRIBUTOR_REG_GICR_PIDR2: hv_gic_redistributor_reg_t

### Message signaled interrupt (MSI) registers

var HV_GIC_REG_GICM_TYPER: hv_gic_msi_reg_t

var HV_GIC_REG_GICM_SET_SPI_NSR: hv_gic_msi_reg_t

### GIC CPU interface (ICC) registers

var HV_GIC_ICC_REG_AP0R0_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_AP1R0_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_BPR0_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_BPR1_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_CTLR_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_IGRPEN0_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_IGRPEN1_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_PMR_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_RPR_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_SRE_EL1: hv_gic_icc_reg_t

var HV_GIC_ICC_REG_SRE_EL2: hv_gic_icc_reg_t

### GIC virtual CPU interface (ICV) registers

var HV_GIC_ICV_REG_AP0R0_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_AP1R0_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_BPR0_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_BPR1_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_CTLR_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_IGRPEN0_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_IGRPEN1_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_PMR_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_RPR_EL1: hv_gic_icv_reg_t

var HV_GIC_ICV_REG_SRE_EL1: hv_gic_icv_reg_t

### GIC hypervisor virtual interface control (ICH) registers

var HV_GIC_ICH_REG_AP0R0_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_AP1R0_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_EISR_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_ELRSR_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_HCR_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR0_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR10_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR11_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR12_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR13_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR14_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR15_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR1_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR2_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR3_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR4_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR5_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR6_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR7_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR8_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_LR9_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_MISR_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_VMCR_EL2: hv_gic_ich_reg_t

var HV_GIC_ICH_REG_VTR_EL2: hv_gic_ich_reg_t

### Reserved interrupt identifiers

func hv_gic_get_intid(hv_gic_intid_t, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

Gets the interrupt ID for reserved interrupts.

var HV_GIC_INT_MAINTENANCE: hv_gic_intid_t

A register Hypervisor uses to signal virtual Interrupts (vIRQs) that the framework sends to guests running at exception level 2 (EL2).

var HV_GIC_INT_PERFORMANCE_MONITOR: hv_gic_intid_t

A register the framework uses to count GIC related events.

var HV_GIC_INT_EL1_PHYSICAL_TIMER: hv_gic_intid_t

var HV_GIC_INT_EL2_PHYSICAL_TIMER: hv_gic_intid_t

var HV_GIC_INT_EL1_VIRTUAL_TIMER: hv_gic_intid_t

## See Also

### Generic interrupt controllers (GICs)

GIC functions

These functions and registers support the creation and operation of a generic interrupt controller.

