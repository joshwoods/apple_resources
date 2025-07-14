

- Hypervisor
-  HV_GIC_INT_PERFORMANCE_MONITOR 

Global Variable

# HV_GIC_INT_PERFORMANCE_MONITOR

A register the framework uses to count GIC related events.

macOS

``` source
var HV_GIC_INT_PERFORMANCE_MONITOR: hv_gic_intid_t { get }
```

## See Also

### Reserved interrupt identifiers

func hv_gic_get_intid(hv_gic_intid_t, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

Gets the interrupt ID for reserved interrupts.

var HV_GIC_INT_MAINTENANCE: hv_gic_intid_t

A register Hypervisor uses to signal virtual Interrupts (vIRQs) that the framework sends to guests running at exception level 2 (EL2).

var HV_GIC_INT_EL1_PHYSICAL_TIMER: hv_gic_intid_t

var HV_GIC_INT_EL2_PHYSICAL_TIMER: hv_gic_intid_t

var HV_GIC_INT_EL1_VIRTUAL_TIMER: hv_gic_intid_t

